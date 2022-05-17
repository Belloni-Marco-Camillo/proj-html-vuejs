<template>
    <div id="UpFooter" class="d-flex">
        <div class="container-footer d-flex justify-content-around col-8 pt-5">

            <div class="text-start">
                <h3>avada university</h3>
                <div
                    v-for="(item, index) in FooterItems" 
                    :key="index"
                    class="pb-2">
                        <div>{{item.conctat}}</div>
                        <div>{{item.road}}</div>
                        <div>{{item.state}}</div>
                </div>

            </div>

            <div class="text-start col-2">

                <h3>recent post</h3>
                <div
                    v-for="(item, index) in FooterPost"
                    :key="index"
                    >   
                    <div><span>> </span>{{item.title}}</div>
                    <div>{{item.getMonth}}/{{item.getDay}}/{{item.getFullYear}}</div>
                    <hr>
                </div>

            </div>

            <div>
                <div class="text-start pb-3">
                    <h3>courses</h3>
                    <div
                        v-for="(Course, index) in Courses"
                        :key="index"
                        >   
                        <a :href="Course.href"><div>{{Course.title}}</div></a>
                    </div>
                </div>

                <div class="text-start">
                    <h3>admission</h3>
                    <div
                        v-for="(admission, index) in admissions"
                        :key="index"
                        >   
                        <a :href="admission.href"><div>{{admission.title}}</div></a>
                    </div>
                </div>


            </div>

            <div>
                <div class="text-start pb-3">
                    <h3>resources</h3>
                    <div
                        v-for="(resource, index) in resources"
                        :key="index"
                        >   
                        <a :href="resource.href"><div>{{resource.title}}</div></a>
                    </div>
                </div>

                <div class="text-start">
                    <h3>quicklinks</h3>
                    <div
                        v-for="(quicklink, index) in quicklinks"
                        :key="index"
                        >   
                        <a :href="quicklink.href"><div>{{quicklink.title}}</div></a>
                    </div>
                </div>

                

            </div>
        </div>

        <div class="col-2 offset-1 pt-5">
            <h3>UPCOMING EVENTS</h3>
            <div class="d-flex">
                <div class="date-events col-2">
                    <p>fri</p>
                    <p>27</p>
                </div>
                <div class="ditails-events text-start offset-1">
                    <h4>Business Seminar</h4>
                    <p>July 1, 2019 @ 8:00 am, - July 1, 2021 @ 5:00 pm</p>
                    <p>United State</p>
                </div>
            </div>
            <hr>
            <div class="d-flex">
                <div class="date-events col-2">
                    <p>fri</p>
                    <p>27</p>
                </div>
                <div class="ditails-events text-start offset-1">
                    <h4>Polictics Seminar</h4>
                    <p>November 6, 2019 @ 8:00 am, - November 6, 2021 @ 5:00 pm</p>
                    <p>United Kingdom</p>
                </div>
            </div>
            <hr>
            <h5 class="text-start"><a href="#">Vuew More...</a></h5>
        </div>
        
        
    </div>
</template>

<script>
import state from "@/state";
export default {
    name: "UpFooter",
    data() {
        return {
            FooterPost:[],
            FooterItems: [
                {
                    conctat: "Residential Location",
                    road: "9521 Broadsberry Avenue",
                    state: "Paddington RC7 9ZA",
                },
                {
                    conctat: "1.800.458.556",
                },
                {
                    conctat: "info@your-domain.com",
                },
                {
                    conctat: "Monday – Friday:",
                    state:"8:00 AM – 10:00 PM"
                },
            ],
            Courses:[
                {
                title:"Art & Humanities",
                href:"#"
                },
                {
                title:"Business & Management",
                href:"#"
                },
                {
                title:"Engineerig & Technology",
                href:"#"
                },
                {
                title:"Life Sciences & Medicine",
                href:"#"
                },
                {
                title:"Nattural scienses",
                href:"#"
                },
            ],
            admissions:[
                {
                title:"Eligibli",
                href:"#"
                },
                {
                title:"Application",
                href:"#"
                },
                {
                title:"Review Process",
                href:"#"
                },
                {
                title:"How to Apllay",
                href:"#"
                },
            ],
            resources:[
                {
                title:"Campus Directory",
                href:"#"
                },
                {
                title:"Academi Calender",
                href:"#"
                },
                {
                title:"Sport Clubs",
                href:"#"
                },
                {
                title:"Graduate Programs",
                href:"#"
                },
                {
                title:"Faculty & Staff",
                href:"#"
                },
            ],
            quicklinks:[
                {
                title:"University Library",
                href:"#"
                },
                {
                title:"Campus Services",
                href:"#"
                },
                {
                title:"Careers",
                href:"#"
                },
            ],
            list:[{
                title: 'titolo',
                items:[
                    {oggetto:'primo'},
                    {oggetto:'secondo'
                }
                ]
            }
            ]
        };
    },
    mounted() {
        this.FooterPost=state.LastPosts;  
        //console.log(this.FooterPost);
    },
}
</script>

<style lang="scss">
@import "@/assets/scss/StyleFooter.scss";
</style>