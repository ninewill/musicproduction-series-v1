<template>
  <!--main-->
  <div id="main" class="wrap wrap-content">
    <section class="section-block section0">
      <video class="" autoplay muted loop>
        <source src="@/assets/images/video/FINAL.mp4" type="video/mp4" />
      </video>
      <div class="sonic-wrap">
        <div class="sonic">
          <img src="@/assets/images/pic/sonic.gif" alt="圖片" />
        </div>
      </div>
    </section>
    <!--START-->
    <section id="1" class="section-block section1">
      <div class="s-title s1-title">
        <h2 class="h2">START</h2>
      </div>
      <div class="s-content s1-content">
        <div class="s1-content-title-1"></div>
        <ul class="s1-item-1">
          <li>
            <div class="s1-img-1">
              <img src="@/assets/images/pic/pic_01-1_photo.svg" alt="圖片" />
            </div>
            <div class="s1-img-2">
              <img src="@/assets/images/pic/pic_01-1_title.svg" alt="圖片" />
            </div>
            <p class="s1-info">
              零基礎至出片、有基礎至精進技法，用最短時間做出完美成品！
            </p>
          </li>
          <li>
            <div class="s1-img-1">
              <img src="@/assets/images/pic/pic_01-2_photo.svg" alt="圖片" />
            </div>
            <div class="s1-img-2">
              <img src="@/assets/images/pic/pic_01-1_title.svg" alt="圖片" />
            </div>
            <p class="s1-info">
              零基礎至出片、有基礎至精進技法，用最短時間做出完美成品！
            </p>
          </li>
          <li>
            <div class="s1-img-1">
              <img src="@/assets/images/pic/pic_01-3_photo.svg" alt="圖片" />
            </div>
            <div class="s1-img-2">
              <img src="@/assets/images/pic/pic_01-1_title.svg" alt="圖片" />
            </div>
            <p class="s1-info">
              零基礎至出片、有基礎至精進技法，用最短時間做出完美成品！
            </p>
          </li>
        </ul>
        <div class="s1-content-title-2"></div>
        <ul class="s1-item-2">
          <li>
            <div class="s1-img-2">
              <img src="@/assets/images/pic/pic_02-1.svg" alt="圖片" />
            </div>
          </li>
          <li>
            <div class="s1-img-2">
              <img src="@/assets/images/pic/pic_02-2.svg" alt="圖片" />
            </div>
          </li>
          <li>
            <div class="s1-img-2">
              <img src="@/assets/images/pic/pic_02-3.svg" alt="圖片" />
            </div>
          </li>
        </ul>
      </div>
    </section>
    <!--Border Line-->
    <div class="section-block border-line">
      <span></span>
      <span class="radius radius-r"></span>
      <span class="radius radius-l"></span>
      <span></span>
    </div>
    <!--COURSE-->
    <section id="2" class="section-block section2">
      <div class="s-title s2-title">
        <h2 class="h2">COURSE</h2>
      </div>
      <!--COURSE Card-->
      <div class="s-content s2-content">
        <div class="s2-content-cards">
          <div class="card-left card-list">
            <div class="card-tags">
              <div class="leave leave1">Leave.01</div>
              <div class="leave leave2">Leave.02</div>
              <div class="leave leave3">Leave.03</div>
            </div>
            <div class="card-list-nav">
              <a @click="handChangePage(0)" :class="{ active: pageIdx === 0 }">
                <span>音樂製作人</span>
                <span>音樂概論/詞曲創作/歌唱技巧/數位編曲</span>
              </a>
              <a @click="handChangePage(1)" :class="{ active: pageIdx === 1 }">
                <span>詞曲創作</span>
                <span>聽力訓練/填詞技巧/作曲實務/DEMO錄音</span>
              </a>
              <a @click="handChangePage(2)" :class="{ active: pageIdx === 2 }">
                <span>編曲配樂</span>
                <span>樂譜識譜/配器編曲/效果器外掛/混音技法</span>
              </a>
              <a @click="handChangePage(3)" :class="{ active: pageIdx === 3 }">
                <span>錄音室職業歌唱</span>
                <span>發聲呼吸/共鳴咬字/歌唱健診/和聲樂理</span>
              </a>
              <a @click="handChangePage(4)" :class="{ active: pageIdx === 4 }">
                <span>EDM電音製作</span>
                <span>介紹器材/實用樂理/樂曲結構/素材混音</span>
              </a>
              <a @click="handChangePage(5)" :class="{ active: pageIdx === 5 }">
                <span>影視配樂作曲</span>
                <span>術語解釋/配樂解析/影像解讀/過帶混音</span>
              </a>
              <a @click="handChangePage(6)" :class="{ active: pageIdx === 6 }">
                <span>電影動畫配樂創作</span>
                <span>音樂概論/和弦記憶法/作曲風格/創作實務</span>
              </a>
            </div>
          </div>
          <div class="card-right card-page">
            <div class="card-lines">
              <span></span>
              <span></span>
              <span></span>
            </div>
            <div class="card-pages">
              <div class="page1" v-if="pageIdx === 0">
                <div class="mid">
                  <div class="mid-title">
                    <div class="mid-title__left">
                      <div class="mid-title__left-t">
                        <div class="mid-title__left-img">
                          <img
                            src="@/assets/images/pic/pic_03_DigitalMusic.svg"
                            alt="圖片"
                          />
                        </div>
                        <span>音樂製作人</span>
                      </div>
                      <div class="mid-title__left-b">
                        72小時晉升音樂製作人，別再當錄音室助理！
                      </div>
                    </div>
                    <div class="mid-title__right">
                      <span>必學課程</span>
                      <span>72HRS</span>
                    </div>
                  </div>
                  <div class="mid-item">
                    <ul>
                      <li>了解市場</li>
                      <li>樂理概念</li>
                      <li>填詞技巧</li>
                      <li>作曲手法</li>
                      <li>配樂編曲</li>
                      <li>出版引薦</li>
                      <li>版權概念</li>
                      <li>混音實務</li>
                      <li>流行歌唱</li>
                      <li>錄音實戰</li>
                    </ul>
                    <div class="mid-music">
                      <div class="mid-music-title">
                        <div class="mid-music-title__left">
                          <img
                            src="@/assets/images/pic/pic_03_career.svg"
                            alt="圖片"
                          />
                        </div>
                        <p>音樂製作人 / 詞曲創作人 / 出版歌手</p>
                      </div>
                      <div class="music-wrap">
                        <div class="music">
                          <div class="music-img">
                            <img
                              src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                              alt="圖片"
                            />
                          </div>
                          <audio controls>
                            <source src="" type="audio/mpeg" />
                          </audio>
                          <div class="music-info">
                            <img
                              src="@/assets/images/pic/pic_03_text1-1.svg"
                              alt="圖片"
                            />
                          </div>
                        </div>
                        <div class="music">
                          <div class="music-img">
                            <img
                              src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                              alt="圖片"
                            />
                          </div>
                          <audio controls>
                            <source src="" type="audio/mpeg" />
                          </audio>
                          <div class="music-info">
                            <img
                              src="@/assets/images/pic/pic_03_text1-1.svg"
                              alt="圖片"
                            />
                          </div>
                        </div>
                        <div class="music">
                          <div class="music-img">
                            <img
                              src="@/assets/images/pic/pic_03_music01_1x.jpeg"
                              alt="圖片"
                            />
                          </div>
                          <audio controls>
                            <source src="" type="audio/mpeg" />
                          </audio>
                          <div class="music-info">
                            <img
                              src="@/assets/images/pic/pic_03_text1-1.svg"
                              alt="圖片"
                            />
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="course-btn">
                  <a href="javascript:;">觀看完整課綱</a>
                </div>
              </div>
              <div class="page2" v-show="pageIdx === 1">
                <div class="mid">456</div>
              </div>
              <div class="page3" v-show="pageIdx === 2">
                <div class="mid">789</div>
              </div>
              <div class="page4" v-show="pageIdx === 3">
                <div class="mid">789</div>
              </div>
              <div class="page5" v-show="pageIdx === 4">
                <div class="mid">789</div>
              </div>
              <div class="page6" v-show="pageIdx === 5">
                <div class="mid">789</div>
              </div>
              <div class="page7" v-show="pageIdx === 6">
                <div class="mid">789</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!--STUDENT WORKS-->
    <section id="3" class="section-block section3">
      <h1>3</h1>
    </section>
    <!--STUDENT WORKS-->
    <section id="4" class="section-block section4">
      <h1>4</h1>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pageIdx: 0,
    };
  },
  methods: {
    handChangePage: function (idx) {
      this.pageIdx = idx;
    },
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/mixin.scss";
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/reset.scss";

.section-block {
  width: calc(100% - 40px);
  margin: 0 auto;

  @include min-width(768px) {
    width: calc(100% - 80px);
  }

  @include min-width(1024px) {
    width: 935px;
  }

  @include min-width(1440px) {
    width: 1200px;
  }

  @include min-width(1920px) {
    width: 1400px;
  }

  &:first-child {
    margin-top: 0;
  }

  > h1 {
    font-size: 80px;
    color: $color-white;
  }
}

.s-content {
  position: relative;
}

//Border Line
.border-line {
  display: flex;
  flex-wrap: wrap;

  > span {
    display: block;
    width: 50%;
    height: 50px;

    &.radius {
      border-color: $color-primary-1;
      border-width: 1px;
    }

    &.radius-r {
      border-bottom-style: dotted;
      border-right-style: dotted;
      border-bottom-right-radius: 50px;
    }

    &.radius-l {
      border-top-style: dotted;
      border-left-style: dotted;
      border-top-left-radius: 50px;
    }
  }
}

.section0 {
  > video {
    width: 100%;
    height: 100%;
    padding-top: 2rem;
  }

  .sonic-wrap {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;

    .sonic-title {
      width: 50%;
      position: absolute;

      > img {
        width: 100%;
        height: 100%;
      }
    }
  }

  .sonic {
    > img {
      width: 100%;
      object-fit: cover;
    }
  }
}

.section1 {
  margin-top: 5rem;

  .s1-title {
    width: 379px;
    height: 95px;
    margin: 0 auto;
    position: relative;

    .h2 {
      width: 100%;
      height: 100%;
      display: block;
      position: absolute;
      top: 0px;
      left: 0px;
      background: url("@/assets/images/pic/pic_01_START.svg") no-repeat
        center/contain;
      @include hidetext;
    }
  }
  .s1-content {
    margin-top: 8rem;
    position: relative;
    border-top: 1px dashed $color-primary-1;
    border-right: 1px dashed $color-primary-1;
    border-top-right-radius: 50px;
  }
  .s1-content-title-1 {
    position: absolute;
    top: 0;
    margin-top: -7%;
    width: 100%;
    padding-bottom: 12.85%;
    background: url("@/assets/images/pic/pic_01_title.svg") no-repeat;
    background-size: contain;
    background-position: 0 100%;
  }
  .s1-content-title-2 {
    width: 100%;
    padding-bottom: 12.85%;
    background: url("@/assets/images/pic/pic_02_title.svg") no-repeat;
    background-size: contain;
    background-position: 0 100%;
  }
  .s1-item-1 {
    margin-top: 9rem;
    padding-right: 5rem;
    padding-bottom: 5rem;
    display: flex;
    align-items: center;
    justify-content: space-between;

    > li {
      width: 30%;

      .s1-img-1 {
        > img {
          width: 100%;
        }
      }

      .s1-img-2 {
        margin-top: 1rem;

        > img {
          width: 100%;
        }
      }

      .s1-info {
        margin-top: 1rem;
        line-height: 26px;
        font-weight: 400;
        font-size: 18px;
        text-align: center;
        color: $color-white;
      }
    }
  }
  .s1-item-2 {
    position: relative;
    margin-top: 5rem;
    padding-right: 5rem;
    padding-bottom: 5rem;
    display: flex;
    align-items: center;
    justify-content: space-between;

    &:after {
      content: "";
      display: block;
      width: 269px;
      height: 308px;
      position: absolute;
      top: -47%;
      right: 5%;
      background: url("@/assets/images/pic/pic_02-4_people.svg") no-repeat;
      background-size: contain;
      background-position: 50% 50%;

      @include min-width(1440px) {
        width: 210px;
        height: 295px;
        right: 8%;
      }

      @include min-width(1920px) {
        width: 269px;
        height: 308px;
        right: 5%;
      }
    }

    > li {
      width: 30%;
      position: relative;
      z-index: 5;

      &::after {
        content: "";
        width: 50px;
        height: 50px;
        position: absolute;
        top: 50%;
        right: -19%;
        display: block;
        background: url("@/assets/images/pic/pic_02-5_cross.svg") no-repeat;
        background-size: contain;
        background-position: 0 100%;
      }

      &:last-child {
        &::after {
          display: none;
        }
      }

      .s1-img-2 {
        > img {
          width: 100%;
        }
      }
    }
  }
}
.section2 {
  position: relative;

  .s2-title {
    width: 379px;
    height: 95px;
    position: absolute;
    top: 0;
    left: 50%;
    z-index: 1;
    margin-left: -189.5px;
    margin-top: -6rem;

    .h2 {
      width: 100%;
      height: 100%;
      display: block;
      position: absolute;
      top: 0px;
      left: 0px;
      background: url("@/assets/images/pic/pic_03_COURSE.svg") no-repeat
        center/contain;
      @include hidetext;
    }
  }
  .s2-content {
    position: relative;
    border-bottom: 1px dashed $color-primary-1;
    border-left: 1px dashed $color-primary-1;
    border-bottom-left-radius: 50px;
    padding-top: 3rem;
    padding-bottom: 5rem;
  }
  .s1-content-title {
    position: absolute;
    top: 0;
    margin-top: -7%;
    width: 100%;
    padding-bottom: 12.85%;
    background: url("@/assets/images/pic/pic_01_title.svg") no-repeat;
    background-size: contain;
    background-position: 0 100%;
  }

  .s2-content-cards {
    padding-right: 50px;
    padding-left: 100px;
    width: 100%;
    display: flex;
    justify-content: space-between;

    .card-left {
      padding: 35px;
      width: 30%;
      border: 1px solid $color-primary-1;
      border-radius: 16px;
      background: linear-gradient(
        137.1deg,
        rgba(0, 224, 184, 0.1) 14.56%,
        rgba(0, 224, 184, 0.1) 85.34%
      );

      &.card-list {
        .card-tags {
          position: absolute;
          top: 70px;
          left: 30px;

          .leave {
            padding: 0.5rem;
            background-color: $color-black;
            border: 1px solid $color-primary-1;
            color: $color-primary-1;
            font-weight: 700;
            font-size: 20px;

            &.leave1 {
              margin-bottom: 4rem;
            }

            &.leave2 {
              margin-bottom: 22rem;
            }
          }
        }

        .card-list-nav {
          > a {
            width: 58%;
            position: relative;
            margin-right: 0;
            margin-left: auto;
            margin-top: 1rem;
            display: block;
            cursor: pointer;

            &:first-child {
              margin-top: 0;
            }

            &:before,
            &:after {
              content: "";
              position: absolute;
              top: 0;
              left: -50px;
              display: block;
            }

            &:before {
              width: 14px;
              height: 14px;
              border-radius: 50%;
              border: 2px solid $color-primary-1;
              background-color: $color-black;
              z-index: 5;
            }

            &:after {
              left: -42px;
              width: 1px;
              height: 100px;
              background-color: $color-primary-1;
            }

            &:last-child {
              &:after {
                display: none;
              }
            }

            &.active {
              &:before {
                content: "";
                border: 2px solid $color-white;
                background-color: $color-primary-1;
              }
            }

            > span {
              display: block;
              font-weight: 400;
              font-size: 14px;
              color: $color-white;

              &:first-child {
                font-weight: 700;
                font-size: 20px;
                color: $color-primary-1;
              }
            }
          }
        }
      }
    }

    .card-right {
      padding: 45px;
      padding-bottom: 100px;
      width: 68.5%;
      border: 1px solid $color-primary-1;
      border-radius: 16px;
      position: relative;

      .card-lines {
        margin-top: -300px;
        height: 600px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        position: absolute;
        top: 50%;
        left: -35px;

        > span {
          width: 45px;
          height: 16px;
          display: block;
          border-radius: 32px;
          border: 1px solid $color-primary-1;
          background-color: $color-black;
        }
      }
    }
  }

  .card-pages {
    .mid {
      .mid-title {
        display: flex;
        justify-content: space-between;
        align-items: flex-end;

        .mid-title__left {
          width: 60%;

          .mid-title__left-t {
            display: flex;
            align-items: center;

            .mid-title__left-img {
              margin-right: 1rem;

              > img {
                width: 100%;
              }
            }

            > span {
              display: block;
              color: $color-primary-1;
              font-weight: 700;
              font-size: 20px;
            }
          }

          .mid-title__left-b {
            margin-top: 1rem;
            font-weight: 400;
            font-size: 20px;
            color: $color-white;
          }
        }

        .mid-title__right {
          width: 30%;
          display: flex;
          justify-content: end;
          align-items: flex-end;

          > span {
            display: block;
            font-weight: 400;
            font-size: 16px;
            color: $color-primary-1;

            &:nth-child(1) {
              margin-right: 0.5rem;
            }
            &:nth-child(2) {
              font-weight: 800;
              font-size: 30px;
              color: $color-primary-7;
            }
          }
        }
      }

      .mid-item {
        margin-top: 3rem;

        > ul {
          width: 100%;
          display: flex;
          justify-content: space-between;
          flex-wrap: wrap;
          border-bottom: 1px dashed $color-primary-1;

          > li {
            width: 15%;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            margin-right: 1rem;
            margin-bottom: 3rem;
            padding: 0.5rem 0;
            border: 1px solid $color-primary-1;
            border-radius: 10px;
            text-align: center;
            color: $color-white;
            font-size: 16px;

            &:nth-child(5n + 5) {
              margin-right: 0;
            }

            &:nth-child(1),
            &:nth-child(2),
            &:nth-child(3),
            &:nth-child(4) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                right: -35px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }
            &:nth-child(5) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                top: 45px;
                transform: rotate(90deg);
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }

            &:nth-child(6),
            &:nth-child(7),
            &:nth-child(8),
            &:nth-child(9) {
              &:after {
                content: "";
                width: 16px;
                height: 24px;
                display: block;
                position: absolute;
                transform: scaleX(-1);
                right: -35px;
                background: url("@/assets/images/pic/pic_03_arrow.svg")
                  no-repeat center/contain;
              }
            }
          }
        }

        .mid-music {
          margin-top: 2rem;

          .mid-music-title {
            display: flex;
            align-items: center;

            > p {
              margin-left: 0.5rem;
              margin-bottom: 0;
              font-size: 16px;
              color: $color-primary-1;
            }
          }

          .music-wrap {
            display: flex;
            justify-content: space-between;
          }

          .music {
            width: 30%;

            .music-img {
              margin-top: 1rem;

              > img {
                width: 100%;
              }
            }

            audio {
              margin-top: 0.75rem;
              width: 100%;
              height: 30px;
            }

            .music-info {
              margin-top: 1rem;

              > img {
                width: 100%;
              }
            }
          }
        }
      }
    }

    .course-btn {
      position: absolute;
      bottom: -50px;
      left: 50%;
      margin-left: -223.5px;

      > a {
        display: block;
        width: 447px;
        height: 109px;
        background: url("@/assets/images/btn/btn_syllabus_default.svg")
          no-repeat center/contain;
        @include hidetext;
        transition: 0.2s;

        @include min-width(1025px) {
          &:hover {
            background: url("@/assets/images/btn/btn_syllabus_hover.svg")
              no-repeat center/contain;
          }
        }
      }
    }
  }
}
.section3 {
  height: 500px;
}
.section4 {
  height: 500px;
}
</style>