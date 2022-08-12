<template>
  <!--menu-->
  <div class="menu-page">
    <!--menu header-->
    <div class="menu-header">
      <div class="menu-header-m">
        <div class="side-right">
          <div class="side-right-block">
            <div class="menu-btn close-btn">
              <a href="javascript:;" title="menu">menu</a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="menu-page-content">
      <div class="menu-page-left">
        <div class="menu-page-left__bg">
          <img src="@/assets/images/pic/pic_00_photo.jpeg" alt="圖片" />
        </div>
      </div>
      <div class="menu-page-right">
        <div class="mic-icon">
          <img src="@/assets/images/pic/sticker.svg" alt="圖片" />
        </div>
        <div class="menu-title">
          <img src="@/assets/images/pic/pic_00_menutitle.svg" alt="圖片" />
        </div>
        <div class="menu-inner">
          <ol>
            <li class="menu-inner-list1">
              <a class="c-link" href="#1">
                <span>01</span>
                <div class="c-text">
                  <p>零基礎也能上手！</p>
                  <small>新手也能開始的音樂製作養成班</small>
                </div>
              </a>
            </li>
            <li class="menu-inner-list2">
              <a class="c-link" href="#2">
                <span>02</span>
                <div class="c-text">
                  <p>音樂製作養成首選！</p>
                  <small>最值得信賴的教學流程與豐富師資</small>
                </div>
              </a>
            </li>
            <li class="menu-inner-list3">
              <a class="c-link" href="#3">
                <span>03</span>
                <div class="c-text">
                  <p>眼見為憑，百聞不如一見！</p>
                  <small>最優質的學習環境＆學員見證分享</small>
                </div>
              </a>
            </li>
          </ol>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    mounted() {

  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

// * ==========================================================================
// * MENU 區塊
// * ==========================================================================

.menu-page {
  width: 100%;
  height: 100%;
  background-color: $color-primary-1;
  position: fixed;
  z-index: 1000;
}

.menu-header {
  margin-top: 50px;
  width: 100%;
  display: flex;
  justify-content: center;
}

.menu-header-m {
  width: 100%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  margin: 0 auto;
  transition: 0.2s;

  @include min-width(1440px) {
    width: 1200px;
  }

  @include min-width(1920px) {
    width: 1400px;
  }
}

.menu-page-content {
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.menu-page-left {
  width: 40%;

  .menu-page-left__bg {
    width: 38%;
    height: 88vh;
    overflow: hidden;
    position: fixed;
    top: 0;
    left: 0;
    border-radius: 0 0 8rem 0;

    > img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}

.menu-page-right {
  width: 30%;
	margin-left: auto;
	margin-right: 25%;
  margin-top: 2rem;

  .menu-title {
    margin-top: 2rem;

		>img{
			width: 100%;
		}
  }

  .menu-inner {
    margin-top: 30px;

    .c-link {
      display: flex;
      align-items: flex-start;
			padding: 2rem 0;
			position: relative;
			border-bottom: 1px dashed $color-white;

			&:after {
				content: "";
				width: 1.474rem;
				height: 1.474rem;
				position: absolute;
				top: 0;
				bottom: 0;
				right: 2.2rem;
				margin: auto;
				background: url("@/assets/images/pic/pic_00_arrow.svg") no-repeat
            center/contain;
			}

      > span {
        margin-right: 35px;
        display: block;
        font-weight: 400;
        font-size: 1rem;
        color: $color-white;
      }

      .c-text {
        > p {
          font-weight: 700;
          font-size: 24px;
          color: $color-white;
        }

				>small{
					font-weight: 400;
					font-size: 18px;
					color: $color-white;
					opacity: 0.7;
				}
      }
    }
  }
}
</style>