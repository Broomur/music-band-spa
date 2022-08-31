<script>
    export default {
        methods: {
            loadPage(page) {
                this.$parent.loadPage(page);
            }
        }
    }
    </script>
    
    <template>
        <div class="w3-top">
            <div class="w3-bar w3-black w3-card">
                <a class="w3-bar-item w3-button w3-padding-large w3-hide-medium w3-hide-large w3-right" href="javascript:void(0)" onclick="myFunction()" title="Toggle Navigation Menu"><i class="fa fa-bars"></i></a>
                <a href="#" @click="loadPage('home')" class="w3-bar-item w3-button w3-padding-large">HOME</a>
                <a href="#band" @click="loadPage('band')" class="w3-bar-item w3-button w3-padding-large w3-hide-small">BAND</a>
                <a href="#tour" @click="loadPage('tour')" class="w3-bar-item w3-button w3-padding-large w3-hide-small">TOUR</a>
                <a href="#contact" @click="loadPage('contact')" class="w3-bar-item w3-button w3-padding-large w3-hide-small">CONTACT</a>
                <a href="javascript:void(0)" class="w3-padding-large w3-hover-red w3-hide-small w3-right"><i class="fa fa-search"></i></a>
            </div>
        </div>
    
        <div id="navDemo" class="w3-bar-block w3-black w3-hide w3-hide-large w3-hide-medium w3-top" style="margin-top:46px">
            <a href="#band" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">BAND</a>
            <a href="#tour" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">TOUR</a>
            <a href="#contact" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">CONTACT</a>
            <a href="#" class="w3-bar-item w3-button w3-padding-large" onclick="myFunction()">MERCH</a>
        </div>
    </template>