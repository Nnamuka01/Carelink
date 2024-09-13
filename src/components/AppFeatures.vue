<script>
import shield from './icons/shield.png';
import medical from './icons/medical.png';
import counsel from './icons/counsel.png';
import wellness from './icons/wellness.png';
import chart from './icons/chart.png';
import umbrella from './icons/umbrella.png';
import book from './icons/book.png';
import access from './icons/access.png';
import care from './icons/care.png';
import multi from './icons/multi.png';
import quote from './icons/double-quote.png';

export default {
    name: 'AppFeatures',
    data() {
        return {
            shield,
            medical,
            counsel,
            wellness,
            chart,
            umbrella,
            book,
            access,
            care,
            multi,
            quote,
        };
    },    
};
</script>

<template>
    <section class="first-section">
        <div class="left-content">
            <div class="first-div">
                <span class="prv-care">
                    <img :src="shield" alt="Shield Icon"> Preventative care
                </span>
                <h2>Preventative health measures built for you</h2>
            </div>
            <div class="hrc">
                <span class="con">
                    <img :src="counsel" alt="Counsel Icon"> Health Counselling
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
                <span class="well">
                    <img :src="wellness" alt="Wellness Icon"> Wellness Exams
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
                <span class="meds">
                    <img :src="medical" alt="Medical Icon"> Preventative Medications
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
            </div>
        </div>
        <div class="csr">
            <img src="../assets/images/counsel.png" alt="A nurse speaking with her patient">
        </div>
    </section>

    <section class="second-section">
        <div class="car">
            <img src="../assets/images/three.png" alt="3 women jogging and smiling">
        </div>
        <div class="right-content">
            <div class="second-div">
                <span class="prv-care">
                    <img :src="shield" alt="Shield Icon"> Wellness programs
                </span>
                <h2>Activities tailored to improve you</h2>
            </div>
            <div class="hrc">
                <span class="con">
                    <img :src="chart" alt="Chart Icon"> Personalized Health Accessments and Goal Setting
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
                <span class="well">
                    <img :src="umbrella" alt="Umbrella Icon"> Interactive Challenges and Activities
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
                <span class="meds">
                    <img :src="book" alt="Book Icon"> Educational Resources and Workshops
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
            </div>
        </div>
    </section>

    <section class="third-section">
        <div class="left-content">
            <div class="third-div">
                <span class="prv-care">
                    <img :src="shield" alt="Shield Icon"> Specialised Treatment
                </span>
                <h2>Advance care for your special needs</h2>
            </div>
            <div class="hrc">
                <span class="con">
                    <img :src="access" alt="Access Icon"> Access to Expertise and Advanced Techniques
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
                <span class="well">
                    <img :src="care" alt="Care Icon"> Comprehensive Care Planning and Coordination
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
                <span class="meds">
                    <img :src="multi" alt="Multi Icon"> Multi-disciplinary Care Teams
                </span>
                <p>We offer guidance on healthy lifestyle behaviours</p>
            </div>
        </div>
        <div class="cap">
            <img src="../assets/images/nurse.png" alt="A nurse with her laptop">
        </div>
    </section>

    <section class="fourth-section">
        <div class="trs-content">
            <div class="fourth-div">
                <span class="prev-care">
                    <img :src="quote" alt="Double Quote Icon"> Testimonials
                </span>
                <h2>You're in good company</h2>
            </div>
            <div class="carl">
                <h2>Carelink are not just your regular healthcare provider. They are your partner in helping and
                    managing your health.</h2>
            </div>
            <div class="pro">
                <h2>Daniel O.</h2>
                <p>Product Designer, Remita</p>
                <div class="pro-images">
                    <img src="../assets/images/chinero2.png" alt="A lady on orange jacket">
                    <img src="../assets/images/joy2.png" alt="A man on green shirt">
                    <img src="../assets/images/nora2.png" alt="A man standing">
                </div>
            </div>
        </div>
    </section>
</template>


<style scoped>
.first-section {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding: 40px;
    background-color: #b4c9e9;
    max-width: 1200px;
    margin: 0 auto;
    margin-bottom: 40px;
}

.left-content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 70%;
}

.first-div,
.hrc {
    text-align: left;
    margin-bottom: 20px;
}

.prv-care {
    border: 1px solid grey;
    background-color: #fff;
    border-radius: 10px;
    padding: 3px;
    display: flex;
    align-items: center;
    gap: 4px;
    width: fit-content;
    margin-bottom: 10px;
}

.prv-care img {
    width: 16px;
    height: 16px;
}

.hrc span {
    display: flex;
    align-items: center;
    gap: 8px;
    margin-bottom: 10px;
}

.hrc p {
    margin-left: 24px;
    margin-top: -10px;
}

.hrc span img {
    width: 16px;
    height: 16px
}

.well,
.meds {
    margin-top: 10px;
}

.csr {
    flex-shrink: 0;
    width: 30%;
    display: flex;
    justify-content: flex-end;
}

.csr img {
    max-width: 100%;
    height: auto;
}

.second-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px;
    background-color: #b4c9e9;
    max-width: 1200px;
    margin: 0 auto;
    gap: 20px;
    margin-bottom: 40px;
}

.car {
    flex: 1;
    display: flex;
    justify-content: flex-start;
    padding-right: 35%;
}

.car img {
    max-width: 100%; 
    height: auto;
}

.right-content {
    flex: 2;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 100%;
}

.right-content h2,
.right-content span,
.right-content p {
    text-align: left;
    margin-bottom: 10px;
}

.third-section {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding: 40px;
    background-color: rgb(211, 211, 211);
    max-width: 1200px;
    margin: 0 auto;
    margin-bottom: 40px;
}

.cap {
    flex-shrink: 0;
    width: 30%;
    display: flex;
    justify-content: flex-end;
}

.cap img {
    max-width: 100%;
    height: auto;
}

.fourth-section {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px;
    background-color: #b4c9e9;
    max-width: 1200px;
    margin: 0 auto;
    margin-bottom: 40px;
}

.prev-care {
    border: 1px solid grey;
    background-color: #fff;
    border-radius: 10px;
    padding: 3px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 4px;
    width: fit-content;
    margin: 0 auto;
    margin-bottom: 10px;
}

.prev-care img {
    width: 16px;
    height: 16px;
}

.trs-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
}

.fourth-div h2 {
    margin-left: -15px;
}

.carl {
    max-width: 400px;
    padding: 15px 10px;
    background-color: #fff;
    border: 2px solid #dcdcdc;
    border-radius: 15px;
    text-align: center;
    position: relative;
    color: #2c2c2c;
    margin: 20px auto;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.carl::after {
    content: '';
    position: absolute;
    bottom: -15px;
    left: 50%;
    transform: translateX(-50%);
    width: 0;
    height: 0;
    border-width: 10px;
    border-style: solid;
    border-color: #fff transparent transparent transparent;
    /* White triangle */
}

.carl::before {
    content: '';
    position: absolute;
    bottom: -17px;
    left: 50%;
    transform: translateX(-50%);
    width: 0;
    height: 0;
    border-width: 12px;
    border-style: solid;
    border-color: #dcdcdc transparent transparent transparent;
}

.pro {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
}

.pro-images {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-top: 10px;
}

.pro img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
}
</style>


