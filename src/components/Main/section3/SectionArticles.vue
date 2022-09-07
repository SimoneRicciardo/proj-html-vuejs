<template>
  <div class="container-articles">

    <div class="articles-titile">
        <span>Articles and Tips</span>
        <h2>Latest From The Blog</h2>
    </div>

    <div class="articles-img">
        <div class="card-img-art">
            <img src="@/images/120084500_197897808368764_8114555493043279565_n.jpg" alt="">
            <div class="info-card">
                <span>ARTIST</span>
                <p>Brush Stronkes Energize Trees in Paintings</p>
                <div>
                    <span><i class="fa-regular fa-calendar"></i> May 15, 2020</span>
                    <span><i class="fa-regular fa-eye"></i> 688 views</span>
                </div>
            </div>
        </div>

        <div class="img-big">
            <img src="@/images/artist-blog-02-500x680.jpg" alt="">
            <div class="info-img-big">
                <span>ARTIST</span>
                <h2>Connection Between Self-Portraits and Identity</h2>
                <div>
                    <span><i class="fa-regular fa-calendar"></i> May 15, 2020</span>
                    <span><i class="fa-regular fa-eye"></i> 397 views</span>
                </div>
            </div>
        </div>

        <div class="card-img-art img-top">
            <img src="@/images/artist-blog-01-480x356.jpg" alt="">
            <div class="info-card">
                <span>ARTIST</span>
                <p>Pocket-Sized Notebooks Hold Miniature Paintings</p>
                <div>
                    <span><i class="fa-regular fa-calendar"></i> May 15, 2020</span>
                    <span><i class="fa-regular fa-eye"></i> 603 views</span>
                </div>
            </div>
        </div>
        
    </div>

    <div class="articles-link">
        <p>Get into details now? <a href="">View all post <i class="fas fa-arrow-right"></i></a></p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'SectionArticles',
}
</script>

<style lang="scss">
.container-articles{

    background: url(@/images/maxcoach-shape-03.png) right 314px,
                url(@/images/maxcoach-shape-12-150x150.png)960px 250px,
                url(@/images/maxcoach-shape-12-150x150.png)1356px 799px;
    background-size: 2791px 450px, 200px 200px, 200px;
    background-color: rgb(245, 247, 250);
    background-repeat:no-repeat ;

    .articles-titile{
        text-align: center;
        margin: 110px 0;
        padding-top: 100px;
        h2{
            padding-top: 30px;
        }
    }

    .articles-img{
        display: flex;
        justify-content: center;
        align-items: center;

        span{
            font-size: 13px;
        }

        p, h2{
            font-weight: 600;
            padding: 15px 0;
        }

        .img-big{
            position: relative;
            color: white;
            img{
                filter: brightness(0.85)
            }
        }
        .info-img-big{
            position: absolute;
            bottom: 110px;
            left: 30px;
        }

        .card-img-art{
            width: 250px;
            background-color: white;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            display: flex;
            flex-direction: column;
            margin: 0 50px;

            img{
            height: 200px;
            }

            .info-card{
                padding: 15px;
            }
        }
        .img-top{
            transform: translatey(-100px);
        }
    }
    .articles-link{
        text-align: center;
        margin: 110px 0;
        padding-bottom: 100px;
        a{
            text-decoration: none;
            color: orange;
        }
    }
}    

</style>