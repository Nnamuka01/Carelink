<script>
import question from './icons/question-fill.png';
import blog from './icons/news-fill.png';

export default {
    name: 'AppFaq',
    data() {
        return {
            question,
            blog,
            // Array of accordions, each with a title, content, and open state
            accordionItems: [
                {
                    title: 'What is Carelink?',
                    content: 'Carelink is a healthcare provider that allows individuals and organisations to acquire professional healthcare service with ease.',
                    isOpen: true,
                },
                {
                    title: 'Do i need to pay before i opt into Carelink?',
                    content: 'Carelink provides access to healthcare professionals through an online platform or in-person visits so payment comes only when you subscribe.',
                    isOpen: false,
                },
                {
                    title: 'Do i get access to valuable resources?',
                    content: 'Valuable resources are all carelink has to offer to its users and you can access them online or in-person visits as the case may be.',
                    isOpen: false,
                },
                {
                    title: 'How long does it take before i get into the app?',
                    content: 'To get started, simply sign up on our platform and you can have access to the app.',
                    isOpen: false,
                },
                {
                    title: 'Do i have to show up daily?',
                    content: 'It is advisable user visit the app daily so they can always be informed about their health status',
                    isOpen: false,
                },
            ],
        };
    },
    methods: {
        // Toggle the accordion, closing all others
        toggleAccordion(index) {
            this.accordionItems.forEach((item, i) => {
                item.isOpen = i === index ? !item.isOpen : false; // Only toggle the clicked one, close others
            });
        },
    },
};
</script>

<template>
    <section class="faq-section">
        <div class="faq-content">
            <div class="faq-div">
                <span class="faq-care">
                    <img :src="question" alt="Question Icon"> FAQ
                </span>
                <h2>Frequently asked questions</h2>
            </div>
            <div class="accordions">
                <div v-for="(item, index) in accordionItems" :key="index" class="accordion">
                    <div class="accordion-header" @click="toggleAccordion(index)">
                        <h3>{{ item.title }}</h3>
                        <span class="toggle-btn">{{ item.isOpen ? '–' : '+' }}</span>
                    </div>
                    <div class="accordion-content" v-show="item.isOpen">
                        <p>{{ item.content }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="blog-section">
        <div class="blog-content">
            <div class="faq-div">
                <span class="faq-care">
                    <img :src="blog" alt="Blog Icon"> Blogs
                </span>
                <h2>Discover health tips to help you live better.</h2>
            </div>
            <div class="blog-images">
                <div class="image-1">
                    <img src="../assets/images/Frame 451.png" alt="">
                    <h3 style="color: #0461f0;">2 MINS READ</h3>
                    <h3>Top 10 tips to improving your health habit</h3>
                    <p>We offer guidance on healthy lifestyle behaviours</p>
                </div>
                <div class="image-2">
                    <img src="../assets/images/Frame 449 (2).png" alt="">
                    <h3 style="color: #0461f0;">2 MINS READ</h3>
                    <h3>Top 10 tips to improving your health habit</h3>
                    <p>We offer guidance on healthy lifestyle behaviours</p>
                </div>
                <div class="image-3">
                    <img src="../assets/images/Frame 450 (1).png" alt="">
                    <h3 style="color: #0461f0;">2 MINS READ</h3>
                    <h3>Top 10 tips to improving your health habit</h3>
                    <p>We offer guidance on healthy lifestyle behaviours</p> 
                </div>       
            </div>
            <div class="blog-button">
                <a class="bg" href="">Visit blog</a>
            </div>
        </div>
    </section>

    <section class="final-section">
        <div class="final-content">
            <div class="final-div">
                <h2>Open an account for free today</h2>
                <p>Supercharge your health with our health provider and stay at your very best, everytime.</p>
            </div>
            <div class="final-button">
                <a class="free" href="">Open a free accounnt</a>
            </div>
        </div>
    </section>
</template>

<style scoped>
.faq-section {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px;
    max-width: 1200px;
    margin: 0 auto;
    margin-bottom: 40px;
}

.faq-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 70%;
}

.faq-div {
    text-align: center;
    margin-bottom: 20px;
}

.faq-care {
    border: 1px solid grey;
    background-color: #fff;
    border-radius: 10px;
    padding: 3px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 4px;
    margin: 0 auto;
    width: fit-content;
    margin-bottom: 10px;
}

.faq-care img {
    width: 16px;
    height: 16px;
}

.accordion {
  border: 1px solid #ccc;
  margin-bottom: 10px;
  border-radius: 5px;
}

.accordion-header {
  display: flex;
  justify-content: space-between;
  padding: 10px;
  background-color: #f4f4f4;
  cursor: pointer;
}

.accordion-content {
  padding: 10px;
  background-color: #fff;
  border-top: 1px solid #ccc;
}

.toggle-btn {
  font-weight: bold;
}

.blog-images {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    gap: 10px;
    padding: 0px;
    justify-content: center;
}

.image-1, .image-2, .image-3 {
    display: flex;
    flex-direction: column;
    gap: 10px;
    width: 30%;
    height: 30%;
}

.blog-button {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
}

.bg {
    color: black;
    border: 1px;
    background-color: #fff;
    border-radius: 20px;
    padding: 10px;
    padding-inline: 20px;
    margin-bottom: 20px;
}

.bg:hover {
    background-color: #0461f0;
    color: #fff;
}

.final-section {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px;
    max-width: 1200px;
    margin: 0 auto;
    margin-bottom: 40px;
    background-color: #023584;
    border-radius: 20px;
}

.final-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 70%;
}

.final-div {
    text-align: center;
    margin-bottom: 20px;
    color: #fff;
}

.final-div h2 {
    margin-bottom: 20px;
}

.final-button {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
}

.free {
    color: white;
    border: 1px;
    background-color: #0461f0;
    border-radius: 20px;
    padding: 10px;
    padding-inline: 20px;
}

.free:hover {
    background-color: #0056b3;
}
</style>