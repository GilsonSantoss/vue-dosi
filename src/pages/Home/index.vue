<template>
  <div class="container">
    <nav class="navbar">
      <span class="navbar-toggle" id="js-navbar-toggle">
        <img src="../../assets/humberger_1.png" alt="nav hidden icon">
      </span>
      <a href="./index.html" class="logo"><img src="../../assets/logo.png" alt="logo"></a>
      <ul class="main-nav" id="js-menu">
        <li>
          <a href="#" class="nav-links">About</a>
        </li>
        <li>
          <a href="#" class="nav-links">Login</a>
        </li>
        <li>
          <a href="#" class="nav-links">Signup</a>
        </li>
      </ul>
    </nav>

    <header class="home_img">
      <!-- Home image passed in css as background image-->
      <h1>Welcome To The home of medecine</h1>
      <p>with us do not worry anymore, we guarante your life and offer much more</p>
      <a href="#" class="button">Create Account</a>
    </header>

    <!-- Medecine -->
    <h1 class="view_Medecine">Available Medecine</h1>
    <div class="container_Medecine">
      <div class="view_details">
        <img src="../../assets/1.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title A</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
      <div class="view_details">
        <img src="../../assets/2.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title B</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
      <div class="view_details">
        <img src="../../assets/3.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title c</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
      <div class="view_details">
        <img src="../../assets/4.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title D</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
      <div class="view_details">
        <img src="../../assets/5.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title E</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
      <div class="view_details">
        <img src="../../assets/6.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title F</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
      <div class="view_details">
        <img src="../../assets/7.jpg" alt="Medecine">
        <div class="item">
          <p style="text-align: center;">Title G</p>
          <p style="text-align: center;">price - 34.00&dollar;</p>
        </div>
        <hr />
      </div>
    </div>

    <!-- footer -->
    <footer>
      <p>App designed by Eric Niyongabo &#x24B8; 2019</p>
    </footer>
  </div>
</template>

<script>
export default { }
</script>

<style lang="scss" scoped>
  @import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap');

  /* ---------------------------------
      navigation bar
  --------------------------------- */

  .navbar {
    font-size: 18px;
    background-color: #F0948A;
    padding-bottom: 10px;
  }

  .main-nav {
    list-style-type: none;
    display: none;
  }

  .nav-links {
    text-decoration: none;
    color: white;
  }

  .main-nav li {
    text-align: center;
    margin: 15px auto;
  }

  .logo {
    display: inline-block;
    margin-top: 10px;
    margin-left: 20px;
  }

  .navbar-toggle {
    position: absolute;
    top: 10px;
    right: 20px;
    cursor: pointer;
    color: rgba(255, 255, 255, 0.8);
    font-size: 24px;
  }

  .active {
    display: block;
  }

  .nav-links:hover {
    padding: 14px 10px;
    background: black;
  }

  @media screen and (min-width: 768px) {
    .navbar {
      display: flex;
      justify-content: space-between;
      padding-bottom: 0;
      height: 70px;
      align-items: center;
    }
    .main-nav {
      display: flex;
      margin-right: 30px;
      flex-direction: row;
      justify-content: flex-end;
    }
    .main-nav li {
      margin: 0;
    }
    .nav-links {
      padding: 10px;
    }
    .navbar-toggle {
      display: none;
    }
  }

  /* ---------------------------------
      Home page
  --------------------------------- */

  .home_img {
    background-image: url(../../assets/home.jpg);
    background-size: cover;
    background-position: center;
    height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
  }

  .home_img h1 {
    font-size: 50px;
    line-height: 1.2;
    color: white;
  }

  .home_img p {
    font-size: 20px;
    color: #fff;
  }

  .home_img .button {
    font-size: 18px;
    text-decoration: none;
    color: white;
    border: #f0948a 1px solid;
    padding: 10px 20px;
    border-radius: 10px;
    margin-top: 20px;
    background-color: black;
  }

  .home_img .button:hover {
    background: green;
    color: #fff;
  }

  h1.view_Medecine {
    text-align: center;
  }

  /* --------------------
      Available medice
  ----------------------*/

  .container_Medecine {
    font-family: monospace;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  .container_Medecine .view_details {
    width: 200px;
    padding: 0.5rem;
    background-color: white;
    margin: .5rem 0.4rem 1rem 0;
  }

  .container_Medecine .view_details img {
    width: 200px;
    height: 100px;
    margin: 2rem 0;
  }

  .container_Medecine .view_details img:hover {
    opacity: 0.9;
  }

  .container_Medecine a.view_image:hover {
    color: #2A6637;
  }

  .item {
    margin-bottom: 10px;
    font-size: 1rem
  }

  @media screen and (min-width: 300px) and (max-width: 512px) {
    .container_Medecine .view_details {
      width: 100%;
    }
    .container_Medecine .view_details img {
      width: 100%;
      height: auto;
    }
    .container_Medecine .view_details span {
      display: table;
      margin: auto;
    }
  }

  @media screen and (min-width: 1000px) {
    .container_Medecine .view_details {
      padding: 0 1rem;
      height: 15rem;
    }
  }

  /* --------------------
      Footer
  ----------------------*/
  footer {
    text-align: center;
    padding: 40px;
    background-color: #f0948a;
    position: relative;
  }

  a {
    text-decoration: none;
  }

  ul {
    list-style: none;
  }
</style>
