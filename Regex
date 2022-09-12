<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Validation</title>

    <!-- CSS only -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-iYQeCzEYFbKjA/T2uDLTpkwGzCiq6soy8tYaI1GyVh/UjpbCx/TYkiZhlZB6+fzT" crossorigin="anonymous">

<!-- JavaScript Bundle with Popper -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-u1OknCvxWvY5kfmNBILK2hRnQC3Pr17a+RTT6rIHI7NnikvbZlHgTPOOmMi466C8" crossorigin="anonymous"></script>

</head>
<body>
    <h1 class="text-center bg-dark text-white">Form Validation using REGEX</h1>
    <div class="container">
        <br><br>
        <form action="" onsubmit="return validation()">
            <div class="form-group">
                <label for=""> UserName :  </label>
                <input type="text" id="username" class="form-control">
                <span id="usererror" class="text-danger font-weight-bold"></span>
            </div><br>
            <div class="form-group">
                <label for=""> Password :  </label>
                <input type="text" id="password" class="form-control">
                <span id="passworderror" class="text-danger font-weight-bold"></span>
            </div><br>
            <div class="form-group">
                <label for=""> Conform Password :  </label>
                <input type="text" id="cpassword" class="form-control">
                <span id="cpassworderror" class="text-danger font-weight-bold"></span>
            </div><br>
            <div class="form-group">
                <label for=""> Email :  </label>
                <input type="text" id="email" class="form-control">
                <span id="emailerror" class="text-danger font-weight-bold"></span>
            </div>
            <br>
            <div class="form-group">
                <label for=""> Mobile Number :  </label>
                <input type="text" id="number" class="form-control">
                <span id="mobileerror" class="text-danger font-weight-bold"></span>
            </div>
            <br>
            <input type="submit" class="btn btn-primary">
        </form>
    </div>
    <script>
        function validation(){
            var username = document.getElementById('username').value
            // alert('username')
            var password = document.getElementById('password').value
            var cpassword = document.getElementById('cpassword').value
            var email = document.getElementById('email').value
            var number = document.getElementById('number').value
            
            var usercheck = /^[A-Za-z]{3,30}$/gm
            var passwordcheck = /^(?=.*[0-9])(?=.*[!@#$%^&*])[a-zA-Z0-9!@#$%^&*]{8,16}$/gm
            var emailcheck = /[a-zA-Z0-9_.]{3,}@[A-Za-z]{3,}[.]{1}[A-Za-z.]{2,6}/gm
            var mobilecheck = /^[789][0-9]{9}$/gm

            if(usercheck.test(username)){
                document.getElementById('usererror').innerHTML="";
            }
            else{
                document.getElementById('usererror').innerHTML="** User Name is Invalid";
                return false;
            }
            if(passwordcheck.test(password)){
                document.getElementById('passworderror').innerHTML="";
            }
            else{
                document.getElementById('passworderror').innerHTML="** Password is Invalid";
                return false;
            }
            if(cpassword.match(password)){
                document.getElementById('cpassworderror').innerHTML="";
            }
            else{
                document.getElementById('cpassworderror').innerHTML="** Password is not Matching";
                return false;
            }
            if(emailcheck.test(email)){
                document.getElementById('emailerror').innerHTML="";
            }
            else{
                document.getElementById('emailerror').innerHTML="** Email Id is Invalid";
                return false;
            }
            if(mobilecheck.test(number)){
                document.getElementById('mobileerror').innerHTML="";
            }
            else{
                document.getElementById('mobileerror').innerHTML="** Mobile Number is Invalid";
                return false;
            }
            
        }
    </script>
</body>
</html>
