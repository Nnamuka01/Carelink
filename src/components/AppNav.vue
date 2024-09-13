<template>
    <nav class="navabr">
        <div class="nav-inner">
            <div class="nav-logo">
                <img src="../assets/images/Logo(1).png" alt="The Company Logo">
            </div>
            <div class="nav-links">
                <li class="nav-link">
                    <a href="">For Individuals</a>
                </li>
                <li class="nav-link">
                    <a href="">For Organizations</a>
                </li>
                <li class="nav-link">
                    <a href="">Partner with Us</a>
                </li>
            </div>    
                    <div id="nav-btns">
                        <a class="nav-btn" href="">Login</a>
                        <a class="nav-btn0" href="">Get Started</a>
                    </div>
        </div>
    </nav>


</template>

<style scoped>
 nav .nav-inner {
    height: 90%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: calc(1440px - 170px);
    width: 100%;
    margin: auto;
    padding: 20px;
 }

 .nav-links {
    display: flex;
    align-items: center;
 }

 .nav-link {
    list-style-type: none;
    padding: 1px 1px;
 }

 .nav-link a {
    padding: 10px;
    text-decoration: none;
    color: black;
 }

 .nav-link :hover {
    background-color: rgba(0, 0, 0, 0.493);
 }

 #nav-btns {
    display: flex;
    gap: 10px;
    align-items: center;
    justify-content: center;
 }

 #nav-btns a {
    text-decoration: none;
 }

 .nav-btn {
    color: black;
    border: 1px solid gray;
    padding: 7px;
    border: none;
 }

 .nav-btn:hover{
    background-color: #0056b3;
    color: #fff;
 }

  .nav-btn0 {
    color: white;
    border: 1px;
    background-color: #0461f0;
    border-radius: 20px;
    padding: 10px;
    padding-inline: 20px;
 }

 .nav-btn0:hover {
    background-color: #0056b3;
 }

</style>
