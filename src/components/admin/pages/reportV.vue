<template>
    <div>
        <h2>Пользователи университета международного бизнеса</h2>

        <div class="container" id="users_card">
            <div class="row">
                <div class="col-md-4 cards">
                    <div class="card" style="width: 18rem;">
                        <div class="card-body">
                            <!-- <h5 class="card-title">Пользователь с ID {{ item.id }}</h5> -->
                            <p class="card-text">
                                78537453245
                                345wefwefwefwefwef
                            </p>
                            <!-- <p class="card-text">Возраст: {{ item.age }}</p> -->
                            <!-- <RouterLink :to="'/user-data?lastName=' + item.lastName + '&firstName=' + item.firstName
                    + '&age=' + item.age + '&exp=' + item.exp + '&degree=' + item.degree + '&endUniversity=' + item.endUniversity
                    + '&position=' + item.position
                    ">
                                ...
                            </RouterLink> -->
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- <UserModal :choosenUser="choosenUser" @change_user="changeUser" /> -->
</template>

<!-- <script>
import UserModal from "@/components/users/UserModal.vue";

export default {
    name: "InfoUsers",
    components: {
        UserModal
    },
    props: {
        items: Array,
    },
    data() {
        return {
            checkedUsers: [],
            inputDisabled: false,
            isOpened: false,
            choosenUser: {}
        }
    },
    watch: {
        checkedUsers() {
            if (this.checkedUsers.length > 1) {
                this.inputDisabled = true
            } else {
                this.inputDisabled = false
            }
        },
    },
    methods: {
        changeUserPosition() {
            if (this.checkedUsers.length <= 1) {
                alert("Выберите 2 пользователей")
            } else {
                this.$emit('change_user_position', this.checkedUsers)
                this.checkedUsers = []
            }
        },
        openModal() {
            this.isOpened = true
            this.choosenUser = this.items[this.checkedUsers[0]]
        },
        changeUser(newUsersData) {
            this.$emit('parent_change_user', newUsersData)
        },
        openModalSingle(item) {
            this.choosenUser = item
        }
    }
}
</script> -->

<style scoped>
#users,
#users_action {
    margin-top: 2%;
}

#users_action button {
    margin-left: 2%;
}

#users_card {
    margin-top: 2%;
}

.cards {
    margin-bottom: 2%;
}
</style>