# Virtual_Doctor.com
<!DOCTYPE html>
<html>
<head>
<title>Login Page</title>
<meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
  <script>
    function validateForm() {
      let x = document.forms["loginform"]["email"].value;
      if (x == "") {
        alert("Email must be filled out");
        return false;
      }
      let y = document.forms["loginform"]["pswd"].value;
      if (y == "") {
        alert("Password must be filled out");
        return false;
      }
    }
    </script>
  <style>
    body { background-image: url(https://media.istockphoto.com/photos/doctor-in-blue-background-picture-id1204550097?k=6&m=1204550097&s=170667a&w=0&h=u9egwZbyA057C65xYAl3qOhLJqKyS16RS4fTgdXxX7I=);
        background-repeat: no-repeat;
        background-size: cover;}
  </style>
</head>
<body>
<div>
<div class="container mt-3">
  <h1><center>Login</center></h1><br><br>
  <form name="loginform" action="/action_page.php" onsubmit="return validateForm()" method="post">
    <div class="mb-3 mt-3">
      <label for="email"><b>Email:</b></label><br>
      <input type="email" class="form-control" id="email" placeholder="Enter email" name="email">
    </div>
    <div class="mb-3">
      <label for="pwd"><b>Password:</b></label>
      <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd">
    </div>
    <div class="form-check mb-3">
      <label class="form-check-label">
        <input class="form-check-input" type="checkbox" name="remember"> Remember me
      </label>
      <br><br>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </form>
</div>

</body>
</html>
