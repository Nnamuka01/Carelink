<script>
import linkedin from './icons/linkedin.png';
import facebook from './icons/facebook.png';
import instagram from './icons/Instagram(2).png';
import youtube from './icons/youtube.png';

export default {
    name: 'AppFooter',
    data() {
        return {
            linkedin,
            facebook,
            instagram,
            youtube,
        };
    },
};
</script>

<template>
    <footer class="footer-heading">
        <div class="container">
            <div class="row">
                <div class="footer-row">
                    <img src="../assets/images/Logo(1).png" alt="The Company Logo">
                    <div class="social-links">
                        <a href=""><img :src="linkedin" alt="Our Linkedin"></a>
                        <a href=""><img :src="facebook" alt="Our Facebook"></a>
                        <a href=""><img :src="instagram" alt="Our Instagram"></a>
                        <a href=""><img :src="youtube" alt="Our Youtube"></a>
                    </div>
                </div>
                <div class="footer-row">
                    <h4>Solutions</h4>
                    <ul>
                        <li><a href="" class="">For Individuals</a></li>
                        <li><a href="" class="">For Organizations</a></li>
                    </ul>
                </div>
                <div class="footer-row">
                    <h4>Company</h4>
                    <ul>
                        <li><a href="" class="">About Us</a></li>
                        <li><a href="" class="">What we do</a></li>
                        <li><a href="" class="">Careers</a></li>
                        <li><a href="" class="">Blogs</a></li>
                    </ul>
                </div>
                <div class="footer-row">
                    <h4>Resource</h4>
                    <ul>
                        <li><a href="" class="">Testimonials</a></li>                        
                        <li><a href="" class="">Contact Us</a></li>                        
                        <li><a href="" class="">FAQs</a></li>                        
                        <li><a href="" class="">Privacy Policy</a></li>                        
                        <li><a href="" class="">Terms & Conditions</a></li>                        
                    </ul>
                </div>
            </div>         
        </div>
        <div class="copyright">
            <p>Copyright ©2024, Designed by Daniel Osonuga and Developed by Nnamuka Chukwuka</p>
        </div>
    </footer>
</template>

<style scoped>
.container {
    gap: 20px;
    padding: 20px;
    margin: 0 auto;
    max-width: 1200px;
    background-color: #fff;
    border-radius: 20px;
}

.row {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: space-between;
}

.footer-heading li {
    list-style-type: none;    
}

.footer-heading {
    padding: 50px 15px;
}

.footer-row h4{
    font-size: 18px;
    color: #000;
    text-transform: capitalize;
    margin-bottom: 30px;
    font-weight: 500;
    position: relative;    
}

.footer-row h4::before {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 0;
    width: 50px;
    height: 2px;
    background-color: #0461f0;
}

.footer-row ul li:not(:last-child) {
    margin-bottom: 10px;
}

.footer-row ul li a {
    text-decoration: none;
    color: #bbb;
    font-size: 16px;
    font-weight: 300;
    text-transform: capitalize;
    transition: all 0.3s ease;
    display: block;
}

.footer-row ul li a:hover {
    color: #0461f0;
    padding-left: 8px;
}

.social-links img {
    width: 30px;
    height: 30px;
    margin-right: 10px;
}

.social-links a {
    display: inline-block;
    height: 40px;
    width: 40px;
    margin: 0 10px 10px 0; 
    text-align: center;
    line-height: 40px;
    transition: all 0.5s ease;
}

.social-links a:hover {
    background-color: #0461f0;
}

.copyright {
    text-align: center;
    padding: 20px;
    color: #000;
    border-radius: 20px;
    margin-top: 20px;
}

.copyright p {
    font-size: 16px;
    font-weight: 300;
}
</style>