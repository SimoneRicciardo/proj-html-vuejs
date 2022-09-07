<template>
<div>
    
    <div class="Events-titile">
        <span>Upcoming Events</span>
        <p>Let's Work Together</p>
    </div>

    <div class="container-card">
        <div v-for="(events, index) in eventsList1" :key="index" class="card-events">
            <img :src='"@/images/artist-event-" + events.img + "-250x300.jpg"' alt="">
            <div class="info-card-events">
                <span>{{events.date}}</span>
                <p>{{events.title}}</p>
                <span><i class="fa-sharp fa-solid fa-location-dot"></i>{{events.location}}</span>
            </div>
        </div>
        <div v-for="(events, index) in eventsList2" :key="index" class="card-events card-reverse">
            <img :src='"@/images/artist-event-" + events.img + "-250x300.jpg"' alt="">
            <div class="info-card-events">
                <span>{{events.date}}</span>
                <p>{{events.title}}</p>
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
.Events-titile{
    text-align: center;
    margin: 110px 0;
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
            p{
                padding: 15px 0;
            }
        }
    }
}

</style>