<template>
    <div class="curvy-bg">
        <div class="about col-12 col-sm-10 col-lg-8 pt-5 mx-auto">
            <h1>About Me</h1>
            <p>
                Hi, I'm a Web Developer, passionate about creating and developing web interfaces.
            </p>
            <p>
                I am available for your Freelance Coding Jobs or Full, Part Time Jobs in your Company!
               
            </p>
            <p>
                I am really good at Front End eg.(HTML,CSS,Javascript) and Back End Programming eg.(PHP,SQL,Phython) Coding as well.
            </p>
            <p class="m-0">
                Apart from coding all day and night, sport, cooking and meeting up with friends are my Hobbys!
            </p>
        </div>
    </div>
</template>

<script>
import loader from '@/mixins/loader';

export default {
    mixins: [loader]
};
</script>

<style lang="scss">
.about {
    h1 {
        font-weight: bold;
    }

    p {
        line-height: 2em;
        white-space: wrap;
        span.code {
            white-space: nowrap;
            background: #313131;
            padding: 0.1em 0.4em;
        }
        a {
            color: #1be66c;
            white-space: nowrap;
        }
    }
}

// to keep svg above bottom nav in mobile-view
.mobile-view {
    .about::before {
        background-position: 0px calc(100% - 60px);
    }
}
</style>
