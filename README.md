<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>registration form </title>
</head>
<body>
    <style>
        body{
            background-image: url(back3.jpg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size:100% 100%;
            backface-visibility:hidden;
        }
        .required{
            font-size: 23px;
            font-family: Times New Roman;
        }
        .required::after{
                   content: " *";
                   color: red;
                   font-size: 20px;
        }
        input[type=text] {
            width: 100%;
            padding: 12px 20px;
            margin: 8px 0;
            box-sizing: border-box;
            border: 2px solid gray;
            border-radius: 4px;
        }
        input[type=text] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid gray;
  border-radius: 4px;
}
input[type=file] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid gray;
  border-radius: 4px;
}
input[type=tel] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid gray;
  border-radius: 4px;
}
#button{
    background-color:blue;
  border: none;
  color: white;
  padding: 16px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  transition-duration: 0.4s;
  cursor: pointer;
}
#button:hover{
    background-color: white; 
  color: black; 
  border: 2px solid gray;
}
a:link {
  color:darkred;
  background-color: transparent;
  text-decoration: none;
  font-size: 22px;
}

a:visited {
  color: pink;
  background-color: transparent;
  text-decoration: none;
  font-size: 25px
}
    </style>
    <h1 style="text-align: center;"> GYM registration</h1>
    <p style="color: red; font-size: 20px;"> *every information must be filled </p>
    <form>
        <label for="fname" class="required"> first name</label><br>
        <input type="text" id="fname" name="fname"><br>
        <label for="lname" class="required"> last name</label><br>
        <input type="text" id="lname" name="fname"><br>
        <label for="contact" class="required"> phone</label><br>
        <input type="tel" id="number"><br>
        <label for="gender" class="required"> gender</label><br>
        <input type="radio" id="male" name="gender" value="male" style="height:20px; width:20px; vertical-align:middle;" >
        <label for="gender">Male</label><br>
        <input type="radio" id="female" name="gender" value="female" style="height:20px; width:20px; vertical-align: middle;" >
        <label for="gender">female</label><br>
        <input type="radio" id="transgender" name="gender" value="transgender" style="height:20px; width:20px; vertical-align:middle;" >
        <label for="gender">transgender</label><br>
        <input type="radio" id="prefer-not" name="gender" value="prefer-not" style="height:20px; width:20px; vertical-align: middle;" >
        <label for="gender">prefer not to say</label> <br><br>
        <label for="photo" class="required">photo</label><br>
        <input type="file" accept="image/*" id="photo" name="photo"><br>
        <label for="requir" class="required"> do you need a personal trainer?</label><br>
        <input type="radio" id="yes" name="requir" style="height:20px; width:20px; vertical-align: middle;" >
        <label for="requir">yes</label><br>
        <input type="radio" id="no" name="requir" style="height:20px; width:20px; vertical-align: middle;" >
        <label for="requir">no</label><br>
        <label for="membership" class="required"> membership package</label>
        <select id="member" name="membership" style="width: 100%; padding: 12px 20px;margin: 8px 0; border:2px solid gray;margin: 8px 0;box-sizing: border-box;border-radius: 4px;"><br>
            <option value="3-months">3 months trial</option>
            <option value="1-year"> 1 year</option>
            <option value="2">2 Years</option>
        </select><br> 
                <label>
      <input type="checkbox" id="myCheckbox" />
        <a href="terms.html">  I agree to the terms and conditions </a>
    </label>
    <br /><br />
    <button type="submit" id="submitBtn" disabled>Submit</button>
    </div>        
    </form>
    <script>
    const checkbox = document.getElementById('myCheckbox');
    const submitBtn = document.getElementById('submitBtn');

    checkbox.addEventListener('change', () => {
      submitBtn.disabled = !checkbox.checked;
    });
    </script>
</body>
</html>
