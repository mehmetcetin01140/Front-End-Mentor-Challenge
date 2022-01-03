<template>
  <div id="app">
    <div class="mainarea">
      <div class="leftside">
        <div>
          <h2>Get <span>insights</span> that help your business grow.</h2>
          <p>
            Discover the benefits of data analytics and make better decisions
            regarding revenue, customer experience, and overail efficiency.
          </p>
          <div class="left-bottom">
            <div class="bottom-top">
              <h3>10k+</h3>
              <h3>314</h3>
              <h3>12M+</h3>
            </div>
          </div>
          <div class="bottom">
            <h4>COMPANIES</h4>
            <h4>TEMPLATES</h4>
            <h4>QUERIES</h4>
          </div>
        </div>
      </div>
      <div class="rightside">
        <div class="color"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@500&family=Spline+Sans:wght@600&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100&family=Roboto:wght@100&family=Spline+Sans:wght@600&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,300;1,600&family=Roboto:wght@100&family=Spline+Sans:wght@600&display=swap");
$backgroundBlack: rgba(10, 12, 27, 255);
$centerBackground: rgba(28, 25, 56, 255);
.boxsizing {
  width: 50%;
  height: 100%;
}
.flexcenter {
  display: flex;
  justify-content: center;
}
.fonts {
  font-family: "Poppins", sans-serif;
}
body {
  margin: 0px;
  padding: 0px;
  background-color: $backgroundBlack;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;

  .mainarea {
    width: 100%;
    height: 500px;
    background: $centerBackground;
    display: flex;
    border-radius: 8px;

    .leftside {
      @extend .boxsizing;
      @extend .flexcenter;
      font-size: 25px;

      h2 {
        padding: 0px 150px 0px 80px;
        margin: 0px;
        margin-top: 80px;
        color: white;
        font-family: "Roboto", sans-serif;
        font-family: "Spline Sans", sans-serif;

        span {
          color: rgba(164, 94, 216, 255);
        }
      }
      p {
        padding: 30px 120px 0px 80px;
        @extend.fonts;
        font-size: 18px;
        color: rgb(206, 202, 202);
        margin: 0px;
        line-height: 27px;
        margin-bottom: 50px;
      }
      .left-bottom {
        padding: 0px 20px 0px 20px;
        .bottom-top {
          display: flex;
          width: 100%;

          h3 {
            margin: auto;
            color: white;
            margin-top: 30px;
            @extend.fonts;
            font-size: 28px;
            letter-spacing: 2px;
            width: 100px;
          }
        }
      }
      .bottom {
        padding: 0px 20px 0px 20px;
        display: flex;

        h4 {
          width: 100px !important;
          font-size: 13px;
          margin: auto;
          letter-spacing: 3px;
          color: rgb(179, 175, 175);
          @extend.fonts;
          padding: 2px;
        }
      }
    }
    .rightside {
      background: url("./rightimage.jpg") no-repeat;
      background-size: cover;

      border-radius: 0px 8px 8px 0px;

      @extend .boxsizing;
      .color {
        background: #9c43d37e;
        width: 100%;
        height: 100%;
      }
    }
  }
}
@media screen and (max-width: 1200px) {
  h2 {
    font-size: 30px !important;
  }
  h3 {
    font-size: 25px !important;
  }
  h4 {
    font-size: 12px !important;
  }
  p {
    font-size: 17px !important;
  }
}
@media screen and (max-width: 950px) {
  h2 {
    font-size: 25px !important;
    padding-right: 0px !important;
  }
  h3 {
    font-size: 15px !important;
    margin-top: 0px !important;
  }
  h4 {
    font-size: 10px !important;
  }
  p {
    font-size: 15px !important;
  }
}
</style>
