<template>
  <div class="conatiner-footer">
    <div class="container-info-footer">
      <div class="adress">
        <h4>Address</h4>
        <p>382 NE 191st ST # 87394 Miami, FL 33179-3899</p>
        <p>+1(305)547-9909 (9am - 5pm EST,  Monday-Friday)</p>
        <a href="">support@maxcoach.com</a>
        <div class="link-social-footer">
          <a href=""><i class="fa-brands fa-square-facebook"></i></a>
          <a href=""><i class="fa-brands fa-twitter"></i></a>
          <a href=""><i class="fa-brands fa-instagram"></i></a>
          <a href=""><i class="fa-brands fa-linkedin"></i></a>
        </div>
      </div>

      <div class="list-link-footer">
        <ul>
          <h4>Explore</h4>
          <li><a href="">Start here</a></li>
          <li><a href="">Success Story</a></li>
          <li><a href="">Blog</a></li>
          <li><a href="">Courses</a></li>
          <li><a href="">Contact us</a></li>
        </ul>
        <ul>
          <h4>Information</h4>
          <li><a href="">Membership</a></li>
          <li><a href="">Purchase guide</a></li>
          <li><a href="">Privacy policy</a></li>
          <li><a href="">Terms of service</a></li>
        </ul>
      </div>

      <div class="photo-footer">
        <h3>Instagram <a href="">@maxcoach</a></h3>
        <div>
          <img src="@/images/120084500_197897808368764_8114555493043279565_n.jpg" alt="">
          <img src="@/images/120012142_177596140500760_8623485824101406058_n.jpg" alt="">
          <img src="@/images/120099363_364334431619755_7198812647386067017_n.jpg" alt="">
        </div>
      </div>
    </div>

    <div class="copyright-footer">
      <p>2020 Maxcoach. All Rights Reserved</p>
      <a href=""><i class="fa-solid fa-arrow-up"></i></a>
        
    </div>
  </div>
</template>

<script>
export default {
    name: 'AppFooter',
}
</script>

<style lang="scss">
.conatiner-footer{
  margin: 100px 0;
  .container-info-footer, .list-link-footer{
    display: flex;
    justify-content: center;
    
    a{
      text-decoration: none;
      color: rgb(106, 106, 107);
    }
    .adress{
      p{
        padding: 10px 0;
      }
    }
    .link-social-footer{
      padding: 15px 0;
      a{
        padding-right: 5px;
      }
    }
    ul{
      padding:0 60px ;

      h4{
        padding-bottom: 10px;
      }
      
      li{
        list-style: none;
        padding: 10px  0;
        a{
          text-decoration: none;
          color: rgb(106, 106, 107);
        }
      }
    }
  
    img{
      width: 200px;
      padding: 5px;
    }
  }
  .photo-footer{
    padding:0 25px;
    a{
      color: orange;
    }
    img{
      padding-top: 20px;
    }
  }
  .copyright-footer{
    color: rgb(106, 106, 107);
    text-align: center;
    padding-top: 60px;
    i{
      float: right;
      background-color: rgb(239, 111, 49);
      padding: 16px 18px;
      border-radius:50% ;
      font-size: 18px;
      color: white;
    }
  }
}

</style>