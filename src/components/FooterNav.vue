<template>
    <footer>
        <div class="container h-100">
            <div id="nav" class="row_aligned h-100">
                <div class="row_basic secondary_color_text">
                    <ul>
                        <li><h4>DC COMICS</h4></li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <li><h4>Shop</h4></li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                    <ul>
                        <li><h4>DC</h4></li>
                        <li>Terms Of Service</li>
                        <li>Privacy policy</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certifications</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <li><h4>Sites</h4></li>
                        <li>DC</li>
                        <li>MAD Megazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss" scoped>
/* Navigation properties */
footer {
    background-image: url('../assets/img/footer-bg.jpg');
    height: 300px;
    overflow: hidden;
    ul {
        margin-right: 20px;
        color: gray;
    }
    li {
        font-size: 12px;
        margin: 5px 0;
    }
    h4 {
        margin: 10px 0;
        color: white;
    }
    img {
        height: 120%;
    }
}
</style>
