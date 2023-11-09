<template>
    <footer>
        
        <div class="container">
            <div class="row ">
                <div class="d-flex justify-content-between ">
                <div class="col-5">
                    <div class="row">
                        <div class="col-4">
                            <ul>
                                <h4 class="text-uppercase text-light ">dc comics</h4>
                                <li v-for =" comic in comics" class="text-light">{{comic}}</li>
                            </ul>
                            <ul>
                                <h4 class="text-uppercase text-light">shop</h4>
                                <li v-for =" shopEl in shop" class="text-light">{{shopEl}}</li>
                            </ul>
                        </div>
        
                        <div class="col-4">
                            
                            <ul>
                                <h4 class="text-uppercase text-light">dc</h4>
                                <li v-for ="dcEl in dc" class="text-light">{{dcEl}}</li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <ul>
                                <h4 class="text-uppercase text-light">sites</h4>
                                <li v-for ="sitesEl in sites" class="text-light">{{sitesEl}}</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-7 d-flex justify-content-end">
                    <img src="/src/assets/images/dc-logo-bg.png" alt="dc-logo-bg">
                </div>
            </div>
            </div>  
        </div>
  
</footer>
</template>

<script>
    export default {
        name: 'FooterApp',

        data(){
            return {
                comics:[
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Video',
                    'News'
                ],
                shop:[
                    'shop DC',
                    'Shop DC Collectibles'
                ],

                dc:[
                    'Terms Of Use',
                    'Privacy policy (New)',
                    'Ad Choice',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us'
                ],

                sites:[
                    'DC',
                    'MAD Magazine',
                    'DC Kids',
                    'DC Universe',
                    'DC Power Visa'
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>