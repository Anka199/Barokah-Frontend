<template>
    <div>
 <div class="container">
        <div class="main-content mt-5">
            <div class="container">
                <div class="login-area">
                    <div class="row mb-4">
                        <div class="mx-auto row">
                            <div id="logo">
                                <img src="../../assets/Vector.png" alt="">
                            </div>
                            <div id="brand">
                                <strong>Blanja Barokah</strong>
                            </div>
                        </div>

                    </div>
                    <h4><strong>Reset Password</strong></h4>
                    <form role="form" id="login-form">
                        <div class="form-group">
                            <input type="email" v-model="email" class="form-control-lg w-100 border-0" placeholder="Email">
                        </div>
                        <button type="submit" id="btn" class="btn text-white" :disabled="!email" data-toggle="modal" data-target="#resetPassword">Reset Password</button>
                        <p class="mt-3 text-center">Don't have a Blanja Barokah account? <a href="#" id="forgot" @click="$emit('register-event')">Register</a></p>
                    </form>
                </div>
            </div>
        </div>
    </div>
    <!-- Modal -->
    <div class="modal fade" id="resetPassword" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="modal-body">
                    <!-- ... -->
        <div class="main-content mt-5">
            <div class="container">
                <div class="login-area">
                    <div class="row">
                        <div class="mx-auto row">
                            <div id="logo">
                                <img src="../../assets/Vector.png" alt="">
                            </div>
                            <div id="brand">
                                <strong>Blanja Barokah</strong>
                            </div>
                        </div>
                    </div>
                    <h4 class="m-5"><strong>Request to reset your Account password</strong></h4>
                        <div class="row mb-5">
                            <img src="../../assets/lock 1.png" class="mx-auto">
                        </div>
                        <p class="text-center">The following is the button for you to reset the password.</p>
                        <div class="row">
                        <button type="submit" id="btn" class="btn text-white w-50 mb-4 mx-auto" @click="$emit('confirm-event')">Change Password</button>
                    </div>
                </div>
            </div>
        </div>
                    <!-- ... -->
                </div>
            </div>
        </div>
    </div>
    <!-- Modal -->
    </div>
</template>

<script>
export default {
  name: 'reset',
  data () {
    return {
      email: ''
    }
  },
  computed: {
  }
}
</script>

<style scoped>

</style>
