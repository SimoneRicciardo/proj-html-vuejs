<template>
  <div class="container-paintings">
    <div class="title-paintings">
        <span>Artist coaching</span>
        <h2>Latest Online Courses</h2>
    </div>

    <div class="container-card-paintings">
        <div class="card-paintings" v-for="(paintings, index) in paintingsList" :key="index">
            <img :src='"@/images/artist-course-" + paintings.img + "-480x480.jpg"' alt="">
            <div class="description-card">
                <span class="price">{{paintings.price}}</span>
                <h4 class="title">{{paintings.title}}</h4>
                <div>
                    <a>
                        <i class="fa-solid fa-file-lines"></i>{{paintings.lessons}} Lessons
                    </a>
                    <a>
                        <i class="fa-regular fa-user"></i>{{paintings.students}} Students
                    </a>
                </div>
            </div>
        </div>
    </div>

    <div class="btn-paintings">
        <button class="btn btn-light-orange">View all courses</button>
    </div>
    
  </div>
</template>

<script>
export default {
    name: 'SectionPaintings',
    data(){
        return{
            paintingsList: [
                {
                    img: '08',
                    price: '$18.00',
                    title: 'The Acrylic Painting Academy',
                    lessons: '4',
                    students: '50'
                },
                {
                    img: '07',
                    price: '$21.00',
                    title: 'Drawing and Shading: Complete Course',
                    lessons: '14',
                    students: '50'
                },
                {
                    img: '06',
                    price: '$19.00',
                    title: 'The Color Theory for Digital Artist',
                    lessons: '7',
                    students: '50'
                },
                {
                    img: '05',
                    price: '$35.00',
                    title: 'Ultimate Guide to Digital Sketching for Beginner',
                    lessons: '14',
                    students: '50'
                },
                {
                    img: '04',
                    price: '$19.00',
                    title: 'Portrait Drawing The Smart Way',
                    lessons: '2',
                    students: '50'
                },
                {
                    img: '03',
                    price: '$19.00',
                    title: 'Mastering Watercolor Painting from Beginner',
                    lessons: '9',
                    students: '50'
                },
                {
                    img: '02',
                    price: '$25.00',
                    title: 'The Art & Science of Drawing',
                    lessons: '4',
                    students: '50'
                },
                {
                    img: '01',
                    price: '$22.00',
                    title: 'The Colored Pencil Drawing Course',
                    lessons: '6',
                    students: '50'
                }
            ]
        }
    }
}
</script>

<style lang="scss">

.container-paintings{

    background: url(@/images/artist-shape-01-600x577.png) -164px 434px,
                url(@/images/artist-shape-01-600x577.png) right 10px;
    background-repeat: no-repeat;

    .title-paintings{
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        margin: 90px 0;
    
        h2{
            padding-top:20px ;
        }
    }
    
    .container-card-paintings{
    
        width: 1700px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
    
        .card-paintings{
            display: flex;
            flex-direction: column;
            width: calc(100%/4);
            padding: 25px;
    
            .description-card{
                padding: 15px;
                display: flex;
                flex-direction: column;
                h4, span{
                    padding: 10px 0;
                }
                a{
                    font-size: 13px;
                    color: rgb(106, 106, 107);
                    i{
                        padding: 0 10px;
                    }
                }
            }
    
            .price{
                color: rgb(255, 123, 0) ;
                font-weight: 800;
            }
        }
    }
    .btn-paintings{
        display: flex;
        justify-content: center;
        padding-top: 55px;
    }
}

</style>