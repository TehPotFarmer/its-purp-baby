html, body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  background-color: transparent;
  color: #fff;
}

.achievement-banner, .achievement-banner-big {
  position: absolute;
  bottom: 10px;
  left: calc(50% - 50px);
  width: 100px;
  height: 100px;
  border-radius: 50px;
  background-color: transparent;
  overflow: hidden;
}

.achievement-banner.animated, .animated.achievement-banner-big {
  -webkit-animation: mainAnimationFrames linear 7.5s;
  animation: mainAnimationFrames linear 7.5s;
  -webkit-animation-delay: 0.5s;
  animation-delay: 0.5s;
  -webkit-animation-iteration-count: 1;
  animation-iteration-count: 1;
  -webkit-transform-origin: 50% 50%;
  transform-origin: 50% 50%;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
  /*when the spec is finished*/
}

.achievement-banner-big {
  width: 600px;
  left: calc(50% - 300px);
  background-color: #6441a5;
}

.achievement-banner .achievement-loader, .achievement-banner-big .achievement-loader, .achievement-banner .achievement-trophy, .achievement-banner-big .achievement-trophy {
  width: 100px;
  height: 100px;
  position: absolute;
  top: 0;
  left: 0;
  border-radius: 50px;
  background-color: #4b307b;
  -webkit-animation: achievementLoaderAnimationFrames ease 9s;
  animation: achievementLoaderAnimationFrames ease 9s;
  -webkit-animation-iteration-count: 1;
  animation-iteration-count: 1;
  -webkit-transform: scaleX(0) scaleY(0);
  transform: scaleX(0) scaleY(0);
  -webkit-transform-origin: 50% 50%;
  transform-origin: 50% 50%;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
  /*when the spec is finished*/
}

.achievement-banner .achievement-loader:nth-of-type(1), .achievement-banner-big .achievement-loader:nth-of-type(1), .achievement-banner .achievement-trophy:nth-of-type(1), .achievement-banner-big .achievement-trophy:nth-of-type(1) {
  background-color: #4b307b;
  -webkit-animation-duration: 10s;
  animation-duration: 10s;
}

.achievement-banner .achievement-loader:nth-of-type(2), .achievement-banner-big .achievement-loader:nth-of-type(2), .achievement-banner .achievement-trophy:nth-of-type(2), .achievement-banner-big .achievement-trophy:nth-of-type(2) {
  background-color: #6441a5;
  -webkit-animation-delay: 0.25s;
  animation-delay: 0.25s;
  -webkit-animation-duration: 9.5s;
  animation-duration: 9.5s;
}

.achievement-banner .achievement-loader:nth-of-type(3), .achievement-banner-big .achievement-loader:nth-of-type(3), .achievement-banner .achievement-trophy:nth-of-type(3), .achievement-banner-big .achievement-trophy:nth-of-type(3) {
  background-color: #6034b1;
  -webkit-animation-delay: 0.5s;
  animation-delay: 0.5s;
  -webkit-animation-duration: 9s;
  animation-duration: 9s;
}

.achievement-banner .achievement-loader:nth-of-type(4), .achievement-banner-big .achievement-loader:nth-of-type(4), .achievement-banner .achievement-trophy:nth-of-type(4), .achievement-banner-big .achievement-trophy:nth-of-type(4) {
  background-color: #6441a5;
  -webkit-animation-delay: 0.75s;
  animation-delay: 0.75s;
  -webkit-animation-duration: 8.5s;
  animation-duration: 8.5s;
}

.achievement-banner .achievement-loader:nth-of-type(5), .achievement-banner-big .achievement-loader:nth-of-type(5), .achievement-banner .achievement-trophy:nth-of-type(5), .achievement-banner-big .achievement-trophy:nth-of-type(5) {
  background-color: #4b307b;
  -webkit-animation-delay: 1s;
  animation-delay: 1s;
  -webkit-animation-duration: 8s;
  animation-duration: 8s;
}

.achievement-banner .achievement-trophy, .achievement-banner-big .achievement-trophy {
  background-color: #4b307b;
  -webkit-animation: xboxLogoAnimationFrames ease-out 7.5s;
  animation: xboxLogoAnimationFrames ease-out 7.5s;
  -webkit-animation-delay: 1s;
  animation-delay: 1s;
  color: #fff;
  background-color: transparent !important;
}

.achievement-banner .achievement-trophy:before, .achievement-banner-big .achievement-trophy:before {
  font-size: 3em;
  top: 32px;
  left: 20px;
  position: absolute;
}

.achievement-banner .achievement-text, .achievement-banner-big .achievement-text {
  font-size: 2em;
  position: absolute;
  width: 475px;
  top: calc((100px - 50%) - 1.6em);
  left: 105px;
  text-align: center;
  white-space: pre-wrap;
  word-wrap: break-word;
  color: #fff;
}

.achievement-banner .achievement-text .achievement-notification, .achievement-banner-big .achievement-text .achievement-notification {
  position: relative;
  width: 100%;
  -webkit-animation: achievementTextAnimationFrames linear 2s;
  animation: achievementTextAnimationFrames linear 2s;
  -webkit-animation-delay: 2s;
  animation-delay: 2s;
  top: -13px;
  opacity: 0;
  top: -77px;
}

.achievement-banner .achievement-text .achievement-name, .achievement-banner-big .achievement-text .achievement-name {
  position: absolute;
  width: 100%;
  font-size: .8em;
  top: 75px;
  -webkit-animation: achievementNameAnimationFrames linear 4s;
  animation: achievementNameAnimationFrames linear 4s;
  -webkit-animation-delay: 3s;
  animation-delay: 3s;
  opacity: 0;
}

.achievement-banner .achievement-text .achievement-name .xbox-gamerscore, .achievement-banner-big .achievement-text .achievement-name .xbox-gamerscore {
  position: relative;
  top: 5px;
}

@-webkit-keyframes achievementLoaderAnimationFrames {
  0% {
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
  10% {
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  90% {
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  100% {
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
}
@keyframes achievementLoaderAnimationFrames {
  0% {
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
  10% {
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  90% {
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  100% {
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
}
@-webkit-keyframes xboxLogoAnimationFrames {
  0% {
    background-color: transparent !important;
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
  5% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1.2) scaleY(1.2);
    transform: scaleX(1.2) scaleY(1.2);
  }
  10% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  90% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  95% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1.2) scaleY(1.2);
    transform: scaleX(1.2) scaleY(1.2);
  }
  100% {
    background-color: transparent !important;
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
}
@keyframes xboxLogoAnimationFrames {
  0% {
    background-color: transparent !important;
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
  5% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1.2) scaleY(1.2);
    transform: scaleX(1.2) scaleY(1.2);
  }
  10% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  90% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1) scaleY(1);
    transform: scaleX(1) scaleY(1);
  }
  95% {
    background-color: transparent !important;
    -webkit-transform: scaleX(1.2) scaleY(1.2);
    transform: scaleX(1.2) scaleY(1.2);
  }
  100% {
    background-color: transparent !important;
    -webkit-transform: scaleX(0) scaleY(0);
    transform: scaleX(0) scaleY(0);
  }
}
@-webkit-keyframes achievementTextAnimationFrames {
  0% {
    opacity: 0;
    top: -77px;
  }
  40% {
    opacity: 1;
  }
  55% {
    opacity: 1;
    top: -77px;
    right: 0;
  }
  100% {
    opacity: 0;
    top: -138px;
  }
}
@keyframes achievementTextAnimationFrames {
  0% {
    opacity: 0;
    top: -77px;
  }
  40% {
    opacity: 1;
  }
  55% {
    opacity: 1;
    top: -77px;
    right: 0;
  }
  100% {
    opacity: 0;
    top: -138px;
  }
}
@-webkit-keyframes achievementNameAnimationFrames {
  0% {
    opacity: 0;
    top: 75px;
  }
  20% {
    opacity: 1;
    top: 9px;
  }
  90% {
    opacity: 1;
    top: 9px;
    right: 0;
  }
  100% {
    opacity: 0;
    top: 9px;
  }
}
@keyframes achievementNameAnimationFrames {
  0% {
    opacity: 0;
    top: 75px;
  }
  20% {
    opacity: 1;
    top: 9px;
  }
  90% {
    opacity: 1;
    top: 9px;
    right: 0;
  }
  100% {
    opacity: 0;
    top: 9px;
  }
}
@-webkit-keyframes mainAnimationFrames {
  10% {
    background-color: #6441a5;
  }
  15% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
  }
  20% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
  }
  30% {
    width: 600px;
    left: calc(50% - 300px);
  }
  80% {
    width: 600px;
    left: calc(50% - 300px);
  }
  90% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
    background-color: #6441a5;
  }
  95% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
    background-color: transparent;
  }
}
@keyframes mainAnimationFrames {
  10% {
    background-color: #6441a5;
  }
  15% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
  }
  20% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
  }
  30% {
    width: 600px;
    left: calc(50% - 300px);
  }
  80% {
    width: 600px;
    left: calc(50% - 300px);
  }
  90% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
    background-color: #6441a5;
  }
  95% {
    width: 100px;
    height: 100px;
    left: calc(50% - 50px);
    background-color: transparent;
  }
}
