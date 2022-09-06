<template>
<div>
    
    <div class="Events-titile">
        <span>Upcoming Events</span>
        <p>Let's Work Together</p>
    </div>

    <div v-for="(events, index) in eventsList" :key="index" class="card-events">
        <img :src='"@/images/artist-event-" + events.img + "-250x300.jpg"' alt="">
        <div class="info-card-events">
            <span>{{events.date}}</span>
            <p>{{events.title}}</p>
            <span><i class="fa-sharp fa-solid fa-location-dot"></i>{{events.location}}</span>
        </div>
    </div>

</div>
</template>

<script>
export default {
    name: 'sectionEvents',
    data(){
        return{
            eventsList: [
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
            ]
        }
    }
}
</script>

<style lang="scss">
.Events-titile{
    text-align: center;
    margin: 110px 0;
}

.card-events{
    display: flex;
    flex-direction: row;
    align-items: center;

    img{

    }

    .info-card-events{
        padding:0 45px;
        p{
            padding: 15px 0;
        }
    }
}
</style>