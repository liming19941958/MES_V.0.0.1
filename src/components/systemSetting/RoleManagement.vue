<template>
    <div class="role-management-page">
        <el-container>
            <el-header>
                <div class="header-nav">
                    <el-tabs v-model="activeName" @tab-click="handleClick">
                        <el-tab-pane label="角色基础信息" name="first"><div style="height: 100vh">
                                8888888
                            </div></el-tab-pane>
                        <el-tab-pane label="PC可操作权限" name="second"></el-tab-pane>
                        <el-tab-pane label="app可操作权限" name="third"> <div style="height: 100vh">
                            <el-container>
                                <el-aside width="400px">
                                    <div class="rolesListTitle">角色列表</div>
                                    <div class="rolesList">
                                        <div class="rolesListContent">
                                            <el-col :span="12">
                                                <el-menu
                                                        default-active="2"
                                                        class="el-menu-vertical-demo"
                                                        @open="handleOpen"
                                                        @close="handleClose"
                                                        background-color="#EFFFF3"
                                                        text-color="#000000"
                                                        active-text-color="#389DFF">
                                                    <el-submenu index="1">
                                                        <template slot="title">
                                                            <i class="el-icon-location"></i>
                                                            <span>壕玮集团</span>
                                                        </template>
                                                        <el-menu-item-group>
                                                            <el-menu-item index="1-1">主管</el-menu-item>
                                                            <el-menu-item index="1-2">组员</el-menu-item>
                                                            <el-menu-item index="1-3">客户管理员</el-menu-item>
                                                            <el-menu-item index="1-4">客户1</el-menu-item>
                                                            <el-menu-item index="1-5">客户2</el-menu-item>
                                                        </el-menu-item-group>
                                                    </el-submenu>
                                                </el-menu>
                                            </el-col>
                                        </div>
                                    </div>
                                </el-aside>
                                <el-main>
                                    <div class="roleMain">
                                        888
                                    </div>
                                </el-main>
                            </el-container>
                        </div></el-tab-pane>
                    </el-tabs>
                </div>
            </el-header>
        </el-container>

    </div>


</template>

<script>
    export default {
        name: "RoleManagement",
        data(){
            return{
                activeName: 'first',
                showBox:true
            }
        },
        methods: {

            handleOpen(key, keyPath) {
                console.log(key, keyPath);
            },
            handleClose(key, keyPath) {
                console.log(key, keyPath);
            },
            handleClick(tab, event) {
                console.log(tab, event);

            }
        }
    }
</script>

<style scoped lang="scss">


</style>