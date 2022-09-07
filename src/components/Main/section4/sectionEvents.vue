<template>
<div class="container-events">
    
    <div class="Events-titile">
        <span>Upcoming Events</span>
        <h2>Let's Work Together</h2>
    </div>

    <div class="container-card">
        <div v-for="(events, index) in eventsList1" :key="index" class="card-events">
            <img :src='"@/images/artist-event-" + events.img + "-250x300.jpg"' alt="">
            <div class="info-card-events">
                <span>{{events.date}}</span>
                <h4>{{events.title}}</h4>
                <span><i class="fa-sharp fa-solid fa-location-dot"></i>{{events.location}}</span>
            </div>
        </div>
        <div v-for="(events, index) in eventsList2" :key="index" class="card-events card-reverse">
            <img :src='"@/images/artist-event-" + events.img + "-250x300.jpg"' alt="">
            <div class="info-card-events">
                <span>{{events.date}}</span>
                <h4>{{events.title}}</h4>
                <span><i class="fa-sharp fa-solid fa-location-dot"></i>{{events.location}}</span>
            </div>
        </div>
    </div>

</div>
</template>

<script>
export default {
    name: 'sectionEvents',
    data(){
        return{
            eventsList1: [
                {
                    img: '04',
                    date: 'NOV   22, 2020',
                    title: 'Storytelling Workshop',
                    location: 'Texas, US'
                },
                {
                    img: '03',
                    date: 'OCT 10, 2020',
                    title: 'Painting Art Contest 2020',
                    location: 'New York, US'
                },
                
            ],
            eventsList2: [
                {
                    img: '02',
                    date: 'NOV 23, 2020',
                    title: 'International Art Fair 2020',
                    location: 'Hamburg, Germany'
                },
                {
                    img: '01',
                    date: 'DEC 15, 2020',
                    title: 'Street Performance: Call For Artist',
                    location: 'Illinois, US'
                }
            ],   
        }
    }
}
</script>

<style lang="scss">

.container-events{
    background: url(@/images/artist-shape-01-600x577.png) -776px 313px,
                url(@/images/artist-shape-01-600x577.png) right 169px,
                url(@/images/maxcoach-shape-13-150x150.png)right 279px;
    background-size: 954px 773px, 420px, 265px;
    background-repeat:no-repeat ;
    .Events-titile{
        text-align: center;
        margin: 110px 0;
        h2{
            padding-top: 15px;
        }
    }
    .container-card{
        width: 1070px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
    
        .card-reverse{
            flex-direction: row-reverse;
        }
    
        .card-events{
            display: flex;
            align-items: center;
            width: calc(100%/2);
            padding: 25px 10px;
        
            .info-card-events{
                padding:0 45px;
                span{
                    color: rgb(106, 106, 107);
                }
                h4{
                    padding: 15px 0;
                }
            }
        }
    }
}


</style>