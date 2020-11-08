/**
 * Framework7 5.0.5
 * Full featured mobile HTML framework for building iOS & Android apps
 * http://framework7.io/
 *
 * Copyright 2014-2019 Vladimir Kharlampidi
 *
 * Released under the MIT License
 *
 * Released on: October 16, 2019
 */

/*====================
  Core
  ==================== */
:root {
  --f7-theme-color: #007aff;
  --f7-theme-color-rgb: 0, 122, 255;
  --f7-theme-color-shade: #0066d6;
  --f7-theme-color-tint: #298fff;
  --f7-safe-area-left: 0px;
  --f7-safe-area-right: 0px;
  --f7-safe-area-top: 0px;
  --f7-safe-area-bottom: 0px;
  --f7-safe-area-outer-left: 0px;
  --f7-safe-area-outer-right: 0px;
  --f7-device-pixel-ratio: 1;
}
@supports (left: env(safe-area-inset-left)) {
  :root {
    --f7-safe-area-top: env(safe-area-inset-top);
    --f7-safe-area-bottom: env(safe-area-inset-bottom);
  }
  :root .ios-left-edge,
  :root .ios-edges,
  :root .safe-area-left,
  :root .safe-areas,
  :root .popup,
  :root .sheet-modal,
  :root .panel-left {
    --f7-safe-area-left: env(safe-area-inset-left);
    --f7-safe-area-outer-left: env(safe-area-inset-left);
  }
  :root .ios-right-edge,
  :root .ios-edges,
  :root .safe-area-right,
  :root .safe-areas,
  :root .popup,
  :root .sheet-modal,
  :root .panel-right {
    --f7-safe-area-right: env(safe-area-inset-right);
    --f7-safe-area-outer-right: env(safe-area-inset-right);
  }
  :root .no-safe-areas,
  :root .no-safe-area-left,
  :root .no-ios-edges,
  :root .no-ios-left-edge {
    --f7-safe-area-left: 0px;
    --f7-safe-area-outer-left: 0px;
  }
  :root .no-safe-areas,
  :root .no-safe-area-right,
  :root .no-ios-edges,
  :root .no-ios-right-edge {
    --f7-safe-area-right: 0px;
    --f7-safe-area-outer-right: 0px;
  }
}
@media (-webkit-min-device-pixel-ratio: 2), (min-resolution: 2dppx) {
  :root {
    --f7-device-pixel-ratio: 2;
  }
}
@media (-webkit-min-device-pixel-ratio: 3), (min-resolution: 3dppx) {
  :root {
    --f7-device-pixel-ratio: 3;
  }
}
/*====================
  Fonts & Bars
  ==================== */
:root {
  --f7-font-size: 14px;
  /*
  --f7-bars-link-color: var(--f7-theme-color);
  */
  --f7-bars-bg-image: none;
  --f7-bars-translucent-opacity: 0.8;
  --f7-bars-translucent-blur: 20px;
  --f7-bars-shadow-bottom-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25) 0%, rgba(0, 0, 0, 0.08) 40%, rgba(0, 0, 0, 0.04) 50%, rgba(0, 0, 0, 0) 90%, rgba(0, 0, 0, 0) 100%);
  --f7-bars-shadow-top-image: linear-gradient(to top, rgba(0, 0, 0, 0.25) 0%, rgba(0, 0, 0, 0.08) 40%, rgba(0, 0, 0, 0.04) 50%, rgba(0, 0, 0, 0) 90%, rgba(0, 0, 0, 0) 100%);
  --f7-bars-text-color: #000;
  --f7-bars-bg-color: #f7f7f8;
  --f7-bars-bg-color-rgb: 247, 247, 248;
}
:root .theme-dark,
:root.theme-dark {
  --f7-bars-text-color: #fff;
}
.ios {
  --f7-font-family: -apple-system, SF Pro Text, SF UI Text, system-ui, Helvetica Neue, Helvetica, Arial, sans-serif;
  --f7-line-height: 1.4;
  --f7-text-color: #000;
  --f7-bars-border-color: rgba(0, 0, 0, 0.25);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-text-color: #fff;
  --f7-bars-bg-color: #121212;
  --f7-bars-bg-color-rgb: 22, 22, 22;
  --f7-bars-border-color: rgba(255, 255, 255, 0.16);
}
.md {
  --f7-font-family: Roboto, system-ui, Noto, Helvetica, Arial, sans-serif;
  --f7-line-height: 1.5;
  --f7-bars-border-color: transparent;
  --f7-text-color: #212121;
}
.md .theme-dark,
.md.theme-dark {
  --f7-text-color: rgba(255, 255, 255, 0.87);
  --f7-bars-bg-color: #202020;
}
.aurora {
  --f7-font-family: -apple-system, system-ui, Helvetica, Arial, sans-serif;
  --f7-line-height: 1.5;
  --f7-text-color: #000;
  --f7-bars-border-color: rgba(0, 0, 0, 0.2);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-text-color: #fff;
  --f7-bars-bg-color: #202020;
  --f7-bars-border-color: rgba(255, 255, 255, 0.1);
}
/*====================
  Color Themes
  ==================== */
.text-color-primary {
  --f7-theme-color-text-color: var(--f7-theme-color);
}
.bg-color-primary {
  --f7-theme-color-bg-color: var(--f7-theme-color);
}
.border-color-primary {
  --f7-theme-color-border-color: var(--f7-theme-color);
}
.ripple-color-primary {
  --f7-theme-color-ripple-color: rgba(var(--f7-theme-color-rgb), 0.3);
}
:root {
  --f7-color-red: #ff3b30;
  --f7-color-red-rgb: 255, 59, 48;
  --f7-color-red-shade: #ff1407;
  --f7-color-red-tint: #ff6259;
  --f7-color-green: #4cd964;
  --f7-color-green-rgb: 76, 217, 100;
  --f7-color-green-shade: #2cd048;
  --f7-color-green-tint: #6ee081;
  --f7-color-blue: #2196f3;
  --f7-color-blue-rgb: 33, 150, 243;
  --f7-color-blue-shade: #0c82df;
  --f7-color-blue-tint: #48a8f5;
  --f7-color-pink: #ff2d55;
  --f7-color-pink-rgb: 255, 45, 85;
  --f7-color-pink-shade: #ff0434;
  --f7-color-pink-tint: #ff5676;
  --f7-color-yellow: #ffcc00;
  --f7-color-yellow-rgb: 255, 204, 0;
  --f7-color-yellow-shade: #d6ab00;
  --f7-color-yellow-tint: #ffd429;
  --f7-color-orange: #ff9500;
  --f7-color-orange-rgb: 255, 149, 0;
  --f7-color-orange-shade: #d67d00;
  --f7-color-orange-tint: #ffa629;
  --f7-color-purple: #9c27b0;
  --f7-color-purple-rgb: 156, 39, 176;
  --f7-color-purple-shade: #7e208f;
  --f7-color-purple-tint: #b92fd1;
  --f7-color-deeppurple: #673ab7;
  --f7-color-deeppurple-rgb: 103, 58, 183;
  --f7-color-deeppurple-shade: #563098;
  --f7-color-deeppurple-tint: #7c52c8;
  --f7-color-lightblue: #5ac8fa;
  --f7-color-lightblue-rgb: 90, 200, 250;
  --f7-color-lightblue-shade: #32bbf9;
  --f7-color-lightblue-tint: #82d5fb;
  --f7-color-teal: #009688;
  --f7-color-teal-rgb: 0, 150, 136;
  --f7-color-teal-shade: #006d63;
  --f7-color-teal-tint: #00bfad;
  --f7-color-lime: #cddc39;
  --f7-color-lime-rgb: 205, 220, 57;
  --f7-color-lime-shade: #bac923;
  --f7-color-lime-tint: #d6e25c;
  --f7-color-deeporange: #ff6b22;
  --f7-color-deeporange-rgb: 255, 107, 34;
  --f7-color-deeporange-shade: #f85200;
  --f7-color-deeporange-tint: #ff864b;
  --f7-color-gray: #8e8e93;
  --f7-color-gray-rgb: 142, 142, 147;
  --f7-color-gray-shade: #79797f;
  --f7-color-gray-tint: #a3a3a7;
  --f7-color-white: #ffffff;
  --f7-color-white-rgb: 255, 255, 255;
  --f7-color-white-shade: #ebebeb;
  --f7-color-white-tint: #ffffff;
  --f7-color-black: #000000;
  --f7-color-black-rgb: 0, 0, 0;
  --f7-color-black-shade: #000000;
  --f7-color-black-tint: #141414;
}
.color-theme-red {
  --f7-theme-color: #ff3b30;
  --f7-theme-color-rgb: 255, 59, 48;
  --f7-theme-color-shade: #ff1407;
  --f7-theme-color-tint: #ff6259;
}
.color-theme-green {
  --f7-theme-color: #4cd964;
  --f7-theme-color-rgb: 76, 217, 100;
  --f7-theme-color-shade: #2cd048;
  --f7-theme-color-tint: #6ee081;
}
.color-theme-blue {
  --f7-theme-color: #2196f3;
  --f7-theme-color-rgb: 33, 150, 243;
  --f7-theme-color-shade: #0c82df;
  --f7-theme-color-tint: #48a8f5;
}
.color-theme-pink {
  --f7-theme-color: #ff2d55;
  --f7-theme-color-rgb: 255, 45, 85;
  --f7-theme-color-shade: #ff0434;
  --f7-theme-color-tint: #ff5676;
}
.color-theme-yellow {
  --f7-theme-color: #ffcc00;
  --f7-theme-color-rgb: 255, 204, 0;
  --f7-theme-color-shade: #d6ab00;
  --f7-theme-color-tint: #ffd429;
}
.color-theme-orange {
  --f7-theme-color: #ff9500;
  --f7-theme-color-rgb: 255, 149, 0;
  --f7-theme-color-shade: #d67d00;
  --f7-theme-color-tint: #ffa629;
}
.color-theme-purple {
  --f7-theme-color: #9c27b0;
  --f7-theme-color-rgb: 156, 39, 176;
  --f7-theme-color-shade: #7e208f;
  --f7-theme-color-tint: #b92fd1;
}
.color-theme-deeppurple {
  --f7-theme-color: #673ab7;
  --f7-theme-color-rgb: 103, 58, 183;
  --f7-theme-color-shade: #563098;
  --f7-theme-color-tint: #7c52c8;
}
.color-theme-lightblue {
  --f7-theme-color: #5ac8fa;
  --f7-theme-color-rgb: 90, 200, 250;
  --f7-theme-color-shade: #32bbf9;
  --f7-theme-color-tint: #82d5fb;
}
.color-theme-teal {
  --f7-theme-color: #009688;
  --f7-theme-color-rgb: 0, 150, 136;
  --f7-theme-color-shade: #006d63;
  --f7-theme-color-tint: #00bfad;
}
.color-theme-lime {
  --f7-theme-color: #cddc39;
  --f7-theme-color-rgb: 205, 220, 57;
  --f7-theme-color-shade: #bac923;
  --f7-theme-color-tint: #d6e25c;
}
.color-theme-deeporange {
  --f7-theme-color: #ff6b22;
  --f7-theme-color-rgb: 255, 107, 34;
  --f7-theme-color-shade: #f85200;
  --f7-theme-color-tint: #ff864b;
}
.color-theme-gray {
  --f7-theme-color: #8e8e93;
  --f7-theme-color-rgb: 142, 142, 147;
  --f7-theme-color-shade: #79797f;
  --f7-theme-color-tint: #a3a3a7;
}
.color-theme-white {
  --f7-theme-color: #ffffff;
  --f7-theme-color-rgb: 255, 255, 255;
  --f7-theme-color-shade: #ebebeb;
  --f7-theme-color-tint: #ffffff;
}
.color-theme-black {
  --f7-theme-color: #000000;
  --f7-theme-color-rgb: 0, 0, 0;
  --f7-theme-color-shade: #000000;
  --f7-theme-color-tint: #141414;
}
.color-red {
  --f7-theme-color: #ff3b30;
  --f7-theme-color-rgb: 255, 59, 48;
  --f7-theme-color-shade: #ff1407;
  --f7-theme-color-tint: #ff6259;
}
.text-color-red {
  --f7-theme-color-text-color: #ff3b30;
}
.bg-color-red {
  --f7-theme-color-bg-color: #ff3b30;
}
.border-color-red {
  --f7-theme-color-border-color: #ff3b30;
}
.ripple-color-red,
.ripple-red {
  --f7-theme-color-ripple-color: rgba(255, 59, 48, 0.3);
}
.color-green {
  --f7-theme-color: #4cd964;
  --f7-theme-color-rgb: 76, 217, 100;
  --f7-theme-color-shade: #2cd048;
  --f7-theme-color-tint: #6ee081;
}
.text-color-green {
  --f7-theme-color-text-color: #4cd964;
}
.bg-color-green {
  --f7-theme-color-bg-color: #4cd964;
}
.border-color-green {
  --f7-theme-color-border-color: #4cd964;
}
.ripple-color-green,
.ripple-green {
  --f7-theme-color-ripple-color: rgba(76, 217, 100, 0.3);
}
.color-blue {
  --f7-theme-color: #2196f3;
  --f7-theme-color-rgb: 33, 150, 243;
  --f7-theme-color-shade: #0c82df;
  --f7-theme-color-tint: #48a8f5;
}
.text-color-blue {
  --f7-theme-color-text-color: #2196f3;
}
.bg-color-blue {
  --f7-theme-color-bg-color: #2196f3;
}
.border-color-blue {
  --f7-theme-color-border-color: #2196f3;
}
.ripple-color-blue,
.ripple-blue {
  --f7-theme-color-ripple-color: rgba(33, 150, 243, 0.3);
}
.color-pink {
  --f7-theme-color: #ff2d55;
  --f7-theme-color-rgb: 255, 45, 85;
  --f7-theme-color-shade: #ff0434;
  --f7-theme-color-tint: #ff5676;
}
.text-color-pink {
  --f7-theme-color-text-color: #ff2d55;
}
.bg-color-pink {
  --f7-theme-color-bg-color: #ff2d55;
}
.border-color-pink {
  --f7-theme-color-border-color: #ff2d55;
}
.ripple-color-pink,
.ripple-pink {
  --f7-theme-color-ripple-color: rgba(255, 45, 85, 0.3);
}
.color-yellow {
  --f7-theme-color: #ffcc00;
  --f7-theme-color-rgb: 255, 204, 0;
  --f7-theme-color-shade: #d6ab00;
  --f7-theme-color-tint: #ffd429;
}
.text-color-yellow {
  --f7-theme-color-text-color: #ffcc00;
}
.bg-color-yellow {
  --f7-theme-color-bg-color: #ffcc00;
}
.border-color-yellow {
  --f7-theme-color-border-color: #ffcc00;
}
.ripple-color-yellow,
.ripple-yellow {
  --f7-theme-color-ripple-color: rgba(255, 204, 0, 0.3);
}
.color-orange {
  --f7-theme-color: #ff9500;
  --f7-theme-color-rgb: 255, 149, 0;
  --f7-theme-color-shade: #d67d00;
  --f7-theme-color-tint: #ffa629;
}
.text-color-orange {
  --f7-theme-color-text-color: #ff9500;
}
.bg-color-orange {
  --f7-theme-color-bg-color: #ff9500;
}
.border-color-orange {
  --f7-theme-color-border-color: #ff9500;
}
.ripple-color-orange,
.ripple-orange {
  --f7-theme-color-ripple-color: rgba(255, 149, 0, 0.3);
}
.color-purple {
  --f7-theme-color: #9c27b0;
  --f7-theme-color-rgb: 156, 39, 176;
  --f7-theme-color-shade: #7e208f;
  --f7-theme-color-tint: #b92fd1;
}
.text-color-purple {
  --f7-theme-color-text-color: #9c27b0;
}
.bg-color-purple {
  --f7-theme-color-bg-color: #9c27b0;
}
.border-color-purple {
  --f7-theme-color-border-color: #9c27b0;
}
.ripple-color-purple,
.ripple-purple {
  --f7-theme-color-ripple-color: rgba(156, 39, 176, 0.3);
}
.color-deeppurple {
  --f7-theme-color: #673ab7;
  --f7-theme-color-rgb: 103, 58, 183;
  --f7-theme-color-shade: #563098;
  --f7-theme-color-tint: #7c52c8;
}
.text-color-deeppurple {
  --f7-theme-color-text-color: #673ab7;
}
.bg-color-deeppurple {
  --f7-theme-color-bg-color: #673ab7;
}
.border-color-deeppurple {
  --f7-theme-color-border-color: #673ab7;
}
.ripple-color-deeppurple,
.ripple-deeppurple {
  --f7-theme-color-ripple-color: rgba(103, 58, 183, 0.3);
}
.color-lightblue {
  --f7-theme-color: #5ac8fa;
  --f7-theme-color-rgb: 90, 200, 250;
  --f7-theme-color-shade: #32bbf9;
  --f7-theme-color-tint: #82d5fb;
}
.text-color-lightblue {
  --f7-theme-color-text-color: #5ac8fa;
}
.bg-color-lightblue {
  --f7-theme-color-bg-color: #5ac8fa;
}
.border-color-lightblue {
  --f7-theme-color-border-color: #5ac8fa;
}
.ripple-color-lightblue,
.ripple-lightblue {
  --f7-theme-color-ripple-color: rgba(90, 200, 250, 0.3);
}
.color-teal {
  --f7-theme-color: #009688;
  --f7-theme-color-rgb: 0, 150, 136;
  --f7-theme-color-shade: #006d63;
  --f7-theme-color-tint: #00bfad;
}
.text-color-teal {
  --f7-theme-color-text-color: #009688;
}
.bg-color-teal {
  --f7-theme-color-bg-color: #009688;
}
.border-color-teal {
  --f7-theme-color-border-color: #009688;
}
.ripple-color-teal,
.ripple-teal {
  --f7-theme-color-ripple-color: rgba(0, 150, 136, 0.3);
}
.color-lime {
  --f7-theme-color: #cddc39;
  --f7-theme-color-rgb: 205, 220, 57;
  --f7-theme-color-shade: #bac923;
  --f7-theme-color-tint: #d6e25c;
}
.text-color-lime {
  --f7-theme-color-text-color: #cddc39;
}
.bg-color-lime {
  --f7-theme-color-bg-color: #cddc39;
}
.border-color-lime {
  --f7-theme-color-border-color: #cddc39;
}
.ripple-color-lime,
.ripple-lime {
  --f7-theme-color-ripple-color: rgba(205, 220, 57, 0.3);
}
.color-deeporange {
  --f7-theme-color: #ff6b22;
  --f7-theme-color-rgb: 255, 107, 34;
  --f7-theme-color-shade: #f85200;
  --f7-theme-color-tint: #ff864b;
}
.text-color-deeporange {
  --f7-theme-color-text-color: #ff6b22;
}
.bg-color-deeporange {
  --f7-theme-color-bg-color: #ff6b22;
}
.border-color-deeporange {
  --f7-theme-color-border-color: #ff6b22;
}
.ripple-color-deeporange,
.ripple-deeporange {
  --f7-theme-color-ripple-color: rgba(255, 107, 34, 0.3);
}
.color-gray {
  --f7-theme-color: #8e8e93;
  --f7-theme-color-rgb: 142, 142, 147;
  --f7-theme-color-shade: #79797f;
  --f7-theme-color-tint: #a3a3a7;
}
.text-color-gray {
  --f7-theme-color-text-color: #8e8e93;
}
.bg-color-gray {
  --f7-theme-color-bg-color: #8e8e93;
}
.border-color-gray {
  --f7-theme-color-border-color: #8e8e93;
}
.ripple-color-gray,
.ripple-gray {
  --f7-theme-color-ripple-color: rgba(142, 142, 147, 0.3);
}
.color-white {
  --f7-theme-color: #ffffff;
  --f7-theme-color-rgb: 255, 255, 255;
  --f7-theme-color-shade: #ebebeb;
  --f7-theme-color-tint: #ffffff;
}
.text-color-white {
  --f7-theme-color-text-color: #ffffff;
}
.bg-color-white {
  --f7-theme-color-bg-color: #ffffff;
}
.border-color-white {
  --f7-theme-color-border-color: #ffffff;
}
.ripple-color-white,
.ripple-white {
  --f7-theme-color-ripple-color: rgba(255, 255, 255, 0.3);
}
.color-black {
  --f7-theme-color: #000000;
  --f7-theme-color-rgb: 0, 0, 0;
  --f7-theme-color-shade: #000000;
  --f7-theme-color-tint: #141414;
}
.text-color-black {
  --f7-theme-color-text-color: #000000;
}
.bg-color-black {
  --f7-theme-color-bg-color: #000000;
}
.border-color-black {
  --f7-theme-color-border-color: #000000;
}
.ripple-color-black,
.ripple-black {
  --f7-theme-color-ripple-color: rgba(0, 0, 0, 0.3);
}
@font-face {
  font-family: 'framework7-core-icons';
  src: url("data:application/font-woff;charset=utf-8;base64, d09GRgABAAAAAA0sABAAAAAAGRAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABGRlRNAAANEAAAABoAAAAci1jrz0dERUYAAAsIAAAAIwAAACQAfQBXR1BPUwAADOAAAAAuAAAANuAY7+xHU1VCAAALLAAAAbMAAAQuAxQJ5U9TLzIAAAHcAAAASgAAAGBRKF+WY21hcAAAAowAAACIAAABYt6F0cBjdnQgAAADFAAAAAQAAAAEABEBRGdhc3AAAAsAAAAACAAAAAj//wADZ2x5ZgAAA6wAAASlAAAKBIq7ZiloZWFkAAABbAAAADAAAAA2FnYC32hoZWEAAAGcAAAAIAAAACQHgQM9aG10eAAAAigAAABhAAABJC+cAAFsb2NhAAADGAAAAJQAAACURlRI+G1heHAAAAG8AAAAHwAAACAAjwBMbmFtZQAACFQAAAFTAAAC2WC6Sihwb3N0AAAJqAAAAVYAAAJ2B5LxL3jaY2BkYGAA4iKuLVLx/DZfGbiZGEDgZk2iIYz+/+NfL0sa02cgl4MBLA0AJsoLsnjaY2BkYGD6/K+XQY8l7f8PBgaWNAagCArwBACRVQXFeNpjYGRgYPBkkGZgYQABJiBmZACJOTDogQQADdEA3AB42mNgYfzCOIGBlYGB0YcxjYGBwR1Kf2WQZGhhYGBiYGVmgAFGBiQQkOaawtDAoMBQxXjg/wEGPabPjMUwNYwHwEoUGMQAQ7UMZAAAeNpj2M0gyAACqxgGNWAMAGIdID4A5OwD0rOA+BBI7P9PhuNAMSBmSYOK+wKxExCfBWIJoNzZ/z8Y3YBsF6g4kM2UBpFjBNJMb/7/Z9gNZBtDzGY6CzGHCcQHigMA2dAWtwAAAHjaY2BgYGaAYBkGRgYQiAHyGMF8FgYHIM3DwMHABGQrMOgyWDLEM1T9/w8UBfEMgLzE////P/5//f/V/xv+r4eaAAeMbAxwIUYmIMHEgKYAYjUcsDAwsLKxc3BycfPw8jEQA/gZBASFhEVExcQlJKWkZWTl5BUUlZRVVNXUNTQZBgMAAMR+E+gAEQFEAAAAKgAqACoANAA+AEgAUgBcAGYAcAB6AIQAjgCYAKIArAC2AMAAygDUAN4A6ADyAPwBBgEQARoBJAEuATgBQgFMAVYBYAFqAXQBfgGIAZIBnAGmAbIB3gIAAioCPAJSAmQChAKUAqQC1gLsAv4DHgMwA0IDYANyA5YDtAPEA+oD/AQWBEYEZgR4BIoEsgTIBOIFAnja7VXBTyNVGP++Ke106XamnbYztYeVlukMRmWl03ZwLdAIeCCKZgOKXBY2m15Es8S03lpuSzaSGsOGQPZGoomegI0mmwjVC5uNdZPGgzGc8MDG4ImLmyxTvzfTKmX/A7PJe/O995vXN7/3+37fK3AQBIB1nAYX8NC/hXA5t813wV+pLY/7ILft4mgIWy4Guxm8zXvwaW4bGW4EjaBuBHuDy58VCjhtfRtEg3ZDajW70yg4wMbPsefY/x7jzmAuQl/nbBi6qF/A93CWKkyECCgAUsITllPZtJaSw56ElnabuoiKqX8zlctN5e4uTEwsTOCo/6YgLAqLmM9NDQ1NvT/B4CfCTT8DHQ7NH9Ggj0gAyYTIsZ1GUNfS2dSLKKOOiH/4emTf3p5PjvsOxW2OO/TJPb7dPYYeig7n5hHW8Cu6B16gXRRez+ie3gTbQ46EeSXBWBJbzC9pS3z/yPj8/O3rffx3c2Njc6MrS1olwvfN356fHx/u50fnRkfnbF6gwS6d1w0Q4mlLc7dUUjc2MGsHaHE/wQ1cAS99NRJnixQeN6wHVbVeV6u/p53YWgt+/AlvsP1MVFA3qyiqVr2qTrciYPMJafEyaUH3mZkdQaIfJkmZvJdRcyOdnM68u8vOfyg+Qtch04TmjhLsG2HYdzibREY39zfVSkX9np7lZOf7DFFV+NbrZLmi2jpaK10F7gR8LL9JnRYoJmXU1LkelQtIak+XFOC4/H52v93esH6xTtfW0IUpdK2t/blvtl+ZTw/+ha1TtuxZzZhgdP+auMF0Mr6osYCDJGBbszy+g3nw0EThB2g1vqQeLKqEUeh921mzgG+iBgEaMblsrWz3mFlMC/wyL1MXZG+x6EVNYBOGCXyxyNtnhlms0+/ZfwcMYTzizsQjWLcMrJ8Yxrph2JxrGKW8kG5JZLpitAnRx4+jNScQj+bf8CH8iq+CAECZU2QRBSQmZlaZmOsOBLo/doc8V/yCePHzL8Vun/i1F/m8eNEvOGe4hm8RB+Y1chGvb9qJQc0O4HgcZByj3Pmp+oCSd8bhnpa/j2dCM+pr5uTkJ5NbM8PDM8NLH4RmLtFs0hy4MsKQTr2Yw6jIbHvxrPA6xJKFtbZUpRJhnTxJBPKGw/Paplouq3YdrnAFPCElQwDpAJELeBJI52k76Z51754FzVih0G55hJ2dJuzg+hkQOjXPIPMqQvToKFrDluLtmirgp+RXQN4WzqaFhWpVbTd898yE8tS09rhjrgYxAHfQ1i9oDrMi49GjJ3TsJ9+kFBxU08mfpXRIkqyHkVgsZD2UMCRlpI+441gyGTsN19k8zd5yIcxKBq1scboE9/E60zfrePG/Qr7fab/+gHfZG6YekB03Or8fp/tQsz1vW95E49EN6eoPGLbD+buJ3To63UhqsYizFEqlll+as1yd0+AC8wvlwmDJ6E2EzlR1Y/VOo3FndbWcLVOrsOcr2NdoWL818G7FLJfNiv08X7f2N+OZuF5n9Wo9wMEqrrBh2q5bF+PHGcSP1RTlJphxqop1zjitO52USS/Z7bxuAceWrJadPwMy5C2ev+V1rIhXn9HtH4d0614AAAB42q2QvU7DMBSFj9u0EgyIgewe26qJnA79G6nUpQtiyB5S01ht4sqNVFW8DBsbIxtPwcLEzltw7RqJoQNDI135y/G59rkGcIVXMBy/Du49M4R48dzAJT48N5GwW88BQvbsuYVr9um5jbARkpMFF/R357osM/Tw5LmBG7x7buIBX54D9FjtuQXO3jy3Sf/GDBpbHGCgsEKBGpwy5+jSOoBAggn6xCk2yLAkV0llSFmQOyOyeklnKLeLmd4ejFoVNe/kXT4QyaTP0022VKUyfFFkZpOVW7Uk5yM121aJPYUwWGOEiK62LImU4wo7spqslHtt1qMo10ZGKtcVySe9fw1zJ9ZuNTSfdFPFNBfHlOr/EY7+BENSx1S/b4O5ruq5NivJB7HgU34yKunJMBpH9jnOMXhKPkP7yvk4ZbFpYrfa2ZBKs1O64kIksRCCn+HSH1E3hiEAeNptkAlPwkAUhGfAAxAsyCV4/hbjfd+3aWq7SiN0yXY5/rzRhVKhiZs06b5v3rzZhxTG5+cbxH/nyHxECmkUUUYFVdRQxyoaaGIN69jBLvawjwMcGu0xTnCKM5zjApe4wjVucIs73OMBj3jCM17wijemmOYc57nARWaYZY5LzLPAZVosssQVlllhlTXWucoGm1zjOje4yS1u50LhKLdl+zIsuS3RVzKwlf/Z0qNKdgI7nhWztvjQ5l5wlJKD+LZkqPv1Lofmv5hQGpNCwjY/i2uB1P6H7zraNxW3LUMx6rAi83eptewYy6xyPF+OSDnu9uQgsJ2ekspZDKUahwgHflcoOxBDbf0FijS5uK/XLUzeFIHSFEwq+dkRlifaQgtbyV7gzczoKtHPTphZRlcrO8o8m3G8gKlplMcIisk9m5UlphjFcmQW88z4haZeSXZG3r8TK74rAAAAAAAB//8AAnjaY2BkYGDgAWIZIGYCQmYGTQZGBi0GDyCbBSzGAAANdgDVAHjadVJJTgJBFH1FdwKOIKB0lEEGwSDOs+KsaDyDGzYaE+LCEA/gwjMY4zlcegbjEYwLb4HvVwM9hXS6q/q9V/+/+v9DARhGFjWoVrP9gAhMIuh0IIxq3d81icH+I2fqNQJl/CKMJJ5C7dC3YRolow6D+Dwa2EAUeT5ZlLmb4Frkk0Waf2kkqBh38XlYmEKKCptdwpiLnWGOyT4XxSyu8Yg3fOJHmaqsGupWPat39aG+1B+uqE7xndPnM77oMZQ0nufulNG8SieTW7cV0CW0s4xPV+c9vboScj7NQkDjdmcRK2CFukG+bMV5QOGv4CLXQTGE3+3ycUzr7lR8PlfZgUEZzjAaOGv7WusywawHAaZXw2WMBKKJwz3OZLCaMl9V9v+CHpM6epFvVGtKVCX6Xg65G6SQ+McY8vCCyXSv85YyrRZ9W3QV03vbQZx6iZ3sZ5ETJ6xVkfGlgs7UOvwmM8UYXZAeHiZSYx9vOMkveMU+YyT1+Thv7e3FEStU5rkcFZIlx6/UZceHZ7hW6KTKyrlj2Rlr+r4OKve9ZDUlhzNZ23TWQ+yKiNM4dxmdt/APtJZExAB42mNgZGBg4GKQYzBhYMxJLMlj4GBgAYow/P/PAJJhLM6sSoWKfWCAAwDAjgbRAAB42mNgYGBkAIIbCZo5IPpmTaIhjAYAPREFnQAA") format("woff");
  font-weight: 400;
  font-style: normal;
}
@font-face {
  font-family: 'framework7-skeleton';
  src: url("data:application/font-woff;charset=utf-8;base64, d09GRgABAAAAAAYQAA0AAAAAEcQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABGRlRNAAAF9AAAABkAAAAciVvoDU9TLzIAAAGcAAAASwAAAGBRtV1jY21hcAAAAfwAAAC8AAABamglddJjdnQgAAACuAAAAAQAAAAEABEBRGdhc3AAAAXsAAAACAAAAAj //wADZ2x5ZgAAA2wAAACUAAAJjHCzhiRoZWFkAAABMAAAAC4AAAA2ERr/HWhoZWEAAAFgAAAAGgAAACQC8ADFaG10eAAAAegAAAATAAAAtAMAABFsb2NhAAACvAAAAK4AAACuaNBmhG1heHAAAAF8AAAAHwAAACAAmgA5bmFtZQAABAAAAAFQAAACuLf6wytwb3N0AAAFUAAAAJkAAADOCKMIc3jaY2BkYGAA4lUx8ibx/DZfGbiZGEDgRu39AAT9/wAjA+MBIJeDASwNACBICpsAAHjaY2BkYGA88P8Agx6QAQSMYIQCWABQZgK3AAB42mNgZGBgCGPgYGBiAAEQycgAEnNg0AMJAAANJwDUAHjaY2BhZGCcwMDKwMDow5jGwMDgDqW/MkgytDAwMDGwcjLAACMDEghIc01haGBQYKhlPPD/AIMe4wEGB5gaxgNAHgNQjhEA6dgLvQB42mNkYBBkAAJGKB4KAAAOfQAVAHjaY2BgYGaAYBkGRgYQSAHyGMF8FgYPIM3HwMHAxMDGoMSgxWDNEMsQz1D7/z9QXIFBjUGHwRHIT/z////j/w/+3/9/6//N/zeg5iABRjYGuCAjE5BgQlcAdAILK5DBxs7BycXAzcPLxy8gKCQsIiomLiEpBVYjLSMrJ6+gqKSsoqqmrqGppa2jq6dvYGhkbGJqZs5gwWBpZW1ja2fv4Ojk7OLq5u7h6eXt4+vnHxAYFBwSyjDgAABJLiG7ABEBRAAAACoAKgAqADgARgBUAGIAcAB+AIwAmgCoALYAxADYAOYA9AECARABHgEsAToBSAFWAWQBcgGAAY4BnAGqAbgBxgHUAeIB8AH+AgwCGgIoAjYCRAJSAmACbgJ8AooCmAKmArQCwgLQAt4C8gMAAw4DHAMqAzgDRgNUA2IDcAN+A4wDmgOoA7YDxAPSA+AD7gP8BAoEGAQmBDQEQgRQBF4EbAR6BIgEnASqBLgExgAAeNpjYGIQZGBgmMkYysDMwM6gt5GRQd9mEzsLw1ujjWysd2w2MTMBmQwbmUHCrCDhTexsjH9sNjGCxI0FjQXVjQWVBTvK09IYQ/+tFmQ0BprGyMDw/wAjA+MBoJkMooKKgowMDkwM/xgYRuVwyjEhybFDZBXBKv4zQFVBVI6G36jcqNyo3GiZMSo3Kjes8hQAx51w5njapZC9agJBFIXP+EfSBMEXmEoU3GVcBNFWsLEJKbYKhEUnOrjryrggkgfIQ6RMnzZVHiBNijxM6pydHUiRFAEXLvebc8+duXcBXOEFAtXXw41ngQ6ePddwgXfPdYRCeW6gIx49N9EWb55b1L/oFI1Lnq5dV8kCXTx4rqGNV8913OLTcwNdcee5CSmePLeof2CGHHucYGGwxgYFJGdeos8cQWGICQbkGCkSrOjKGJbKgu6EVOoZ7zCuilm+P1mz3hSyt+zLSA0nAxmnycpkxsrFJrFpku3Nis57NpetGkcOYbHFGAEOzJqXao6SY0ebTTJ9zO12HBy2OtVFTvGX66c0d0LhsuVO2m0ScheJKeN/z1beESuRi+pPYJ7vinlu11pGoZJT+cdwVEdBFJSbn7djzLql1/iBlBsidLlcBrG2B8MHlRqGSil51nPfEi6AO3jaXc5ZM4IBAEbhp9RF1FhCRbmyVNYskSXG0CaEQvaf2j/LN112bt6Zc/HOETZiOJAJJmSc15ENmxARFTNpSlzCtBmz5iTNW7AoJR08LFmWlbNi1Zp1G/IKijZt2bZj156SfQcOHSk7dqLi1JlzF6ouXbl241ZNXUNTy522ew8edTx59qKrF3S9edf34dOXbz9+/f0DgycTFgAAAAAAAAH//wACeNpjYGBgZACCGwmaOWC69n4AjAYARC0G1wAAAA==") format("woff");
  font-weight: 300, 400, 500, 600, 700;
  font-style: normal, italic;
}
html,
body,
.framework7-root {
  position: relative;
  height: 100%;
  width: 100%;
  overflow-x: hidden;
}
body {
  margin: 0;
  padding: 0;
  width: 100%;
  background: #fff;
  overflow: hidden;
  -webkit-text-size-adjust: 100%;
  -webkit-font-smoothing: antialiased;
  font-family: var(--f7-font-family);
  font-size: var(--f7-font-size);
  line-height: var(--f7-line-height);
  color: var(--f7-text-color);
}
.theme-dark {
  color: var(--f7-text-color);
}
.framework7-root {
  overflow: hidden;
  box-sizing: border-box;
}
.framework7-initializing *,
.framework7-initializing *:before,
.framework7-initializing *:after {
  transition-duration: 0ms !important;
}
.device-ios,
.device-android {
  cursor: pointer;
}
.device-ios {
  touch-action: manipulation;
}
@media (width: 1024px) and (height: 691px) and (orientation: landscape) {
  html,
  body,
  .framework7-root {
    height: 671px;
  }
}
@media (width: 1024px) and (height: 692px) and (orientation: landscape) {
  html,
  body,
  .framework7-root {
    height: 672px;
  }
}
* {
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  -webkit-touch-callout: none;
}
a,
input,
textarea,
select {
  outline: 0;
}
a {
  cursor: pointer;
  text-decoration: none;
  color: var(--f7-theme-color);
}
.link,
.item-link {
  cursor: pointer;
}
p {
  margin: 1em 0;
}
.disabled {
  opacity: 0.55 !important;
  pointer-events: none !important;
}
html.device-full-viewport,
html.device-full-viewport body {
  height: 100vh;
}
.ios .md-only,
.ios .if-md,
.ios .aurora-only,
.ios .if-aurora,
.ios .if-not-ios,
.ios .not-ios {
  display: none !important;
}
@media (width: 1024px) and (height: 691px) and (orientation: landscape) {
  .ios,
  .ios body,
  .ios .framework7-root {
    height: 671px;
  }
}
@media (width: 1024px) and (height: 692px) and (orientation: landscape) {
  .ios,
  .ios body,
  .ios .framework7-root {
    height: 672px;
  }
}
.md .ios-only,
.md .if-ios,
.md .aurora-only,
.md .if-aurora,
.md .if-not-md,
.md .not-md {
  display: none !important;
}
.aurora .ios-only,
.aurora .if-ios,
.aurora .md-only,
.aurora .if-md,
.aurora .if-not-aurora,
.aurora .not-aurora {
  display: none !important;
}
/* === Statusbar === */
/* === Views === */
.views,
.view {
  position: relative;
  height: 100%;
  z-index: 5000;
  overflow: hidden;
  box-sizing: border-box;
}
.framework7-root > .view,
.framework7-root > .views {
  height: calc(100% - var(--f7-appbar-app-offset, 0px));
}
/* === Pages === */
:root {
  --f7-page-master-width: 320px;
  --f7-page-master-border-color: rgba(0, 0, 0, 0.1);
  --f7-page-master-border-width: 1px;
  --f7-page-swipeback-transition-duration: 300ms;
  /*
  --f7-page-content-extra-padding-top: 0px;
  --f7-page-content-extra-padding-bottom: 0px;
  */
}
.ios {
  --f7-page-transition-duration: 400ms;
  --f7-page-bg-color: #efeff4;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-page-bg-color: #000;
}
.md {
  --f7-page-transition-duration: 250ms;
  --f7-page-bg-color: #fff;
}
.md .theme-dark,
.md.theme-dark {
  --f7-page-bg-color: #121212;
}
.aurora {
  --f7-page-transition-duration: 400ms;
  --f7-page-bg-color: #f3f3f3;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-page-bg-color: #121212;
}
.theme-dark {
  --f7-page-master-border-color: rgba(255, 255, 255, 0.1);
}
.pages {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
}
.page {
  box-sizing: border-box;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  transform: none;
  background-color: var(--f7-page-bg-color);
  z-index: 1;
}
.page.stacked {
  display: none;
}
.page-with-navbar-large-collapsed {
  --f7-navbar-large-collapse-progress: 1;
}
.page-previous {
  pointer-events: none;
}
.page-content {
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  box-sizing: border-box;
  height: 100%;
  position: relative;
  z-index: 1;
  padding-top: calc(var(--f7-page-navbar-offset, 0px) + var(--f7-page-toolbar-top-offset, 0px) + var(--f7-page-subnavbar-offset, 0px) + var(--f7-page-searchbar-offset, 0px) + var(--f7-page-content-extra-padding-top, 0px));
  padding-bottom: calc(var(--f7-page-toolbar-bottom-offset, 0px) + var(--f7-safe-area-bottom) + var(--f7-page-content-extra-padding-bottom, 0px));
}
.page-transitioning,
.page-transitioning .page-shadow-effect,
.page-transitioning .page-opacity-effect {
  transition-duration: var(--f7-page-transition-duration);
}
.page-transitioning-swipeback,
.page-transitioning-swipeback .page-shadow-effect,
.page-transitioning-swipeback .page-opacity-effect {
  transition-duration: var(--f7-page-swipeback-transition-duration);
}
.router-transition-forward .page-next,
.router-transition-backward .page-next,
.router-transition-forward .page-current,
.router-transition-backward .page-current,
.router-transition-forward .page-previous:not(.stacked),
.router-transition-backward .page-previous:not(.stacked) {
  pointer-events: none;
}
.page-shadow-effect {
  position: absolute;
  top: 0;
  width: 16px;
  bottom: 0;
  z-index: -1;
  content: '';
  opacity: 0;
  right: 100%;
  background: linear-gradient(to right, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 10%, rgba(0, 0, 0, 0.01) 50%, rgba(0, 0, 0, 0.2) 100%);
}
.page-opacity-effect {
  position: absolute;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.1);
  width: 100%;
  bottom: 0;
  content: '';
  opacity: 0;
  z-index: 10000;
}
.ios .page-previous {
  transform: translate3d(-20%, 0, 0);
}
.ios .page-next {
  transform: translate3d(100%, 0, 0);
}
.ios .page-previous .page-opacity-effect {
  opacity: 1;
}
.ios .page-previous:after {
  opacity: 1;
}
.ios .page-current .page-shadow-effect {
  opacity: 1;
}
.ios .router-transition-forward .page-next {
  animation: ios-page-next-to-current var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .page-next:before {
  position: absolute;
  top: 0;
  width: 16px;
  bottom: 0;
  z-index: -1;
  content: '';
  opacity: 0;
  right: 100%;
  background: linear-gradient(to right, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 10%, rgba(0, 0, 0, 0.01) 50%, rgba(0, 0, 0, 0.2) 100%);
  animation: ios-page-element-fade-in var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .page-current {
  animation: ios-page-current-to-previous var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .page-current:after {
  position: absolute;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.1);
  width: 100%;
  bottom: 0;
  content: '';
  opacity: 0;
  z-index: 10000;
  animation: ios-page-element-fade-in var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .page-previous {
  animation: ios-page-previous-to-current var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .page-previous:after {
  position: absolute;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.1);
  width: 100%;
  bottom: 0;
  content: '';
  opacity: 0;
  z-index: 10000;
  animation: ios-page-element-fade-out var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .page-current {
  animation: ios-page-current-to-next var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .page-current:before {
  position: absolute;
  top: 0;
  width: 16px;
  bottom: 0;
  z-index: -1;
  content: '';
  opacity: 0;
  right: 100%;
  background: linear-gradient(to right, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0) 10%, rgba(0, 0, 0, 0.01) 50%, rgba(0, 0, 0, 0.2) 100%);
  animation: ios-page-element-fade-out var(--f7-page-transition-duration) forwards;
}
@keyframes ios-page-next-to-current {
  from {
    transform: translate3d(100%, 0, 0);
  }
  to {
    transform: translate3d(0%, 0, 0);
  }
}
@keyframes ios-page-previous-to-current {
  from {
    transform: translate3d(-20%, 0, 0);
  }
  to {
    transform: translate3d(0%, 0, 0);
  }
}
@keyframes ios-page-current-to-previous {
  from {
    transform: translate3d(0, 0, 0);
  }
  to {
    transform: translate3d(-20%, 0, 0);
  }
}
@keyframes ios-page-current-to-next {
  from {
    transform: translate3d(0, 0, 0);
  }
  to {
    transform: translate3d(100%, 0, 0);
  }
}
@keyframes ios-page-element-fade-in {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes ios-page-element-fade-out {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
.md .page-next {
  transform: translate3d(0, 56px, 0);
  opacity: 0;
  pointer-events: none;
}
.md .page-next.page-next-on-right {
  transform: translate3d(100%, 0, 0);
}
.md .router-transition-forward .page-next {
  animation: md-page-next-to-current var(--f7-page-transition-duration) forwards;
}
.md .router-transition-forward .page-current {
  animation: none;
}
.md .router-transition-backward .page-current {
  animation: md-page-current-to-next var(--f7-page-transition-duration) forwards;
}
.md .router-transition-backward .page-previous {
  animation: none;
}
@keyframes md-page-next-to-current {
  from {
    transform: translate3d(0, 56px, 0);
    opacity: 0;
  }
  to {
    transform: translate3d(0, 0px, 0);
    opacity: 1;
  }
}
@keyframes md-page-current-to-next {
  from {
    transform: translate3d(0, 0, 0);
    opacity: 1;
  }
  to {
    transform: translate3d(0, 56px, 0);
    opacity: 0;
  }
}
.aurora .page-next {
  pointer-events: none;
  transform: translate3d(100%, 0px, 0);
}
.aurora .page-next.page-next-on-right {
  transform: translate3d(100%, 0, 0);
}
.aurora .page-previous .page-opacity-effect {
  opacity: 1;
}
.aurora .page-previous:after {
  opacity: 1;
}
.aurora .router-transition-forward .page-next {
  animation: aurora-page-next-to-current var(--f7-page-transition-duration) forwards;
}
.aurora .router-transition-forward .page-current {
  animation: none;
}
.aurora .router-transition-forward .page-current:after {
  position: absolute;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.1);
  width: 100%;
  bottom: 0;
  content: '';
  opacity: 0;
  z-index: 10000;
  animation: aurora-page-element-fade-in var(--f7-page-transition-duration) forwards;
}
.aurora .router-transition-backward .page-current {
  animation: aurora-page-current-to-next var(--f7-page-transition-duration) forwards;
}
.aurora .router-transition-backward .page-previous {
  animation: none;
}
.aurora .router-transition-backward .page-previous:after {
  position: absolute;
  left: 0;
  top: 0;
  background: rgba(0, 0, 0, 0.1);
  width: 100%;
  bottom: 0;
  content: '';
  opacity: 0;
  z-index: 10000;
  animation: aurora-page-element-fade-out var(--f7-page-transition-duration) forwards;
}
@keyframes aurora-page-next-to-current {
  from {
    transform: translate3d(100%, 0, 0);
  }
  to {
    transform: translate3d(0, 0px, 0);
  }
}
@keyframes aurora-page-current-to-next {
  from {
    transform: translate3d(0, 0, 0);
  }
  to {
    transform: translate3d(100%, 0, 0);
  }
}
@keyframes aurora-page-element-fade-in {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes aurora-page-element-fade-out {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
.view:not(.view-master-detail) .page-master-stacked {
  display: none;
}
.view:not(.view-master-detail) .navbar-master-stacked {
  display: none;
}
.view-master-detail .page-master,
.view-master-detail .navbar-master {
  width: var(--f7-page-master-width);
  --f7-safe-area-right: 0px;
  --f7-safe-area-outer-right: 0px;
  border-right: var(--f7-page-master-border-width) solid var(--f7-page-master-border-color);
}
.view-master-detail .page-master-detail,
.view-master-detail .navbar-master-detail {
  width: calc(100% - var(--f7-page-master-width));
  --f7-safe-area-left: 0px;
  --f7-safe-area-outer-left: 0px;
  left: var(--f7-page-master-width);
}
.view-master-detail .page-master {
  z-index: 2;
  transform: none;
  pointer-events: auto;
}
.view-master-detail .page-master:before,
.view-master-detail .page-master:after {
  display: none;
}
.view-master-detail.router-transition .page-master {
  animation: none;
}
.md .router-transition-custom .page-previous,
.ios .router-transition-custom .page-previous,
.aurora .router-transition-custom .page-previous,
.md .router-transition-custom .page-next,
.ios .router-transition-custom .page-next,
.aurora .router-transition-custom .page-next {
  opacity: 1;
  transform: none;
}
.router-transition-f7-circle-forward:after,
.router-transition-f7-circle-backward:after {
  content: '';
  position: absolute;
  left: 50%;
  top: 50%;
  width: 100vmax;
  height: 100vmax;
  margin-left: -50vmax;
  margin-top: -50vmax;
  background: var(--f7-page-bg-color);
  z-index: 100;
}
.router-transition-f7-circle-forward:after {
  transform: scale(0);
  border-radius: 50%;
  animation: f7-circle-circle-in 400ms forwards;
}
.router-transition-f7-circle-forward .page-next {
  opacity: 0 !important;
  transform: scale(0.9) !important;
  animation: f7-circle-next-to-current 300ms forwards;
  animation-delay: 300ms;
  z-index: 150;
}
.router-transition-f7-circle-backward:after {
  animation: f7-circle-circle-out 300ms forwards;
  animation-delay: 350ms;
}
.router-transition-f7-circle-backward .page-current {
  animation: f7-circle-current-to-next 700ms forwards;
  z-index: 150;
}
@keyframes f7-circle-circle-in {
  from {
    transform: scale(0);
    border-radius: 50%;
  }
  50% {
    border-radius: 50%;
  }
  to {
    transform: scale(1);
    border-radius: 0%;
  }
}
@keyframes f7-circle-circle-out {
  from {
    transform: scale(1);
    border-radius: 0%;
  }
  50% {
    border-radius: 50%;
  }
  to {
    transform: scale(0);
    border-radius: 50%;
  }
}
@keyframes f7-circle-next-to-current {
  from {
    transform: scale(0.9);
    opacity: 0;
  }
  40% {
    transform: scale(1.035);
    opacity: 1;
  }
  to {
    transform: scale(1);
    opacity: 1;
  }
}
@keyframes f7-circle-current-to-next {
  from {
    transform: scale(1);
    opacity: 1;
  }
  34% {
    transform: scale(1.035);
    opacity: 1;
  }
  57% {
    transform: scale(0.9);
    opacity: 0;
  }
  to {
    transform: scale(0.9);
    opacity: 0;
  }
}
.router-transition-f7-cover-v-forward,
.router-transition-f7-cover-v-backward {
  background: #000;
  perspective: 1200px;
}
.router-transition-f7-cover-v-forward .page-next {
  animation: f7-cover-v-next-to-current 450ms forwards;
}
.router-transition-f7-cover-v-forward .page-current {
  animation: f7-cover-v-current-to-prev 450ms forwards;
}
.router-transition-f7-cover-v-backward .page-current {
  animation: f7-cover-v-current-to-next 450ms forwards;
}
.router-transition-f7-cover-v-backward .page-previous {
  animation: f7-cover-v-prev-to-current 450ms forwards;
}
@keyframes f7-cover-v-next-to-current {
  from {
    transform: translateY(100%);
  }
  to {
    transform: translateY(0%);
  }
}
@keyframes f7-cover-v-current-to-next {
  from {
    transform: translateY(0%);
  }
  to {
    transform: translateY(100%);
  }
}
@keyframes f7-cover-v-current-to-prev {
  from {
    transform: translateZ(0);
    opacity: 1;
  }
  to {
    transform: translateZ(-300px);
    opacity: 0.5;
  }
}
@keyframes f7-cover-v-prev-to-current {
  from {
    transform: translateZ(-300px);
    opacity: 0.5;
  }
  to {
    transform: translateZ(0);
    opacity: 1;
  }
}
.router-transition-f7-cover-forward,
.router-transition-f7-cover-backward {
  background: #000;
  perspective: 1200px;
}
.router-transition-f7-cover-forward .page-next {
  animation: f7-cover-next-to-current 450ms forwards;
}
.router-transition-f7-cover-forward .page-current {
  animation: f7-cover-current-to-prev 450ms forwards;
}
.router-transition-f7-cover-backward .page-current {
  animation: f7-cover-current-to-next 450ms forwards;
}
.router-transition-f7-cover-backward .page-previous {
  animation: f7-cover-prev-to-current 450ms forwards;
}
@keyframes f7-cover-next-to-current {
  from {
    transform: translateX(100%);
  }
  to {
    transform: translateX(0%);
  }
}
@keyframes f7-cover-current-to-next {
  from {
    transform: translateX(0%);
  }
  to {
    transform: translateX(100%);
  }
}
@keyframes f7-cover-current-to-prev {
  from {
    transform: translateZ(0);
    opacity: 1;
  }
  to {
    transform: translateZ(-300px);
    opacity: 0.5;
  }
}
@keyframes f7-cover-prev-to-current {
  from {
    transform: translateZ(-300px);
    opacity: 0.5;
  }
  to {
    transform: translateZ(0);
    opacity: 1;
  }
}
.router-transition-f7-dive-forward,
.router-transition-f7-dive-backward {
  background: var(--f7-page-bg-color);
  perspective: 1200px;
}
.router-transition-f7-dive-forward .page-next {
  animation: f7-dive-next-to-current 500ms forwards;
}
.router-transition-f7-dive-forward .page-current {
  animation: f7-dive-current-to-prev 500ms forwards;
}
.router-transition-f7-dive-backward .page-current {
  animation: f7-dive-current-to-next 500ms forwards;
}
.router-transition-f7-dive-backward .page-previous {
  animation: f7-dive-prev-to-current 500ms forwards;
}
@keyframes f7-dive-next-to-current {
  from {
    opacity: 0;
    transform: translateZ(-150px);
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 1;
    transform: translateZ(0px);
  }
}
@keyframes f7-dive-current-to-next {
  from {
    opacity: 1;
    transform: translateZ(0px);
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 0;
    transform: translateZ(-150px);
  }
}
@keyframes f7-dive-current-to-prev {
  from {
    transform: translateZ(0px);
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 0;
    transform: translateZ(150px);
  }
}
@keyframes f7-dive-prev-to-current {
  from {
    opacity: 0;
    transform: translateZ(150px);
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 1;
    transform: translateZ(0px);
  }
}
.router-transition-f7-fade-forward,
.router-transition-f7-fade-backward {
  background: var(--f7-page-bg-color);
}
.router-transition-f7-fade-forward .page-next {
  opacity: 0 !important;
  animation: f7-fade-in 500ms forwards;
}
.router-transition-f7-fade-forward .page-current {
  animation: f7-fade-out 500ms forwards;
}
.router-transition-f7-fade-backward .page-current {
  animation: f7-fade-out 500ms forwards;
}
.router-transition-f7-fade-backward .page-previous {
  animation: f7-fade-in 500ms forwards;
}
@keyframes f7-fade-in {
  from {
    opacity: 0;
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes f7-fade-out {
  from {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  to {
    opacity: 0;
  }
}
.router-transition-f7-flip-forward,
.router-transition-f7-flip-backward {
  background: #000;
  perspective: 1200px;
}
.router-transition-f7-flip-forward .page,
.router-transition-f7-flip-backward .page {
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.router-transition-f7-flip-forward .page-next {
  animation: f7-flip-next-to-current 700ms forwards;
}
.router-transition-f7-flip-forward .page-current {
  animation: f7-flip-current-to-prev 700ms forwards;
}
.router-transition-f7-flip-backward .page-current {
  animation: f7-flip-current-to-next 700ms forwards;
}
.router-transition-f7-flip-backward .page-previous {
  animation: f7-flip-prev-to-current 700ms forwards;
}
@keyframes f7-flip-next-to-current {
  from {
    border-radius: 30px;
    transform: translateZ(-100vmax) rotateY(180deg);
  }
  to {
    border-radius: 0;
    transform: translateZ(0px) rotateY(0deg);
  }
}
@keyframes f7-flip-current-to-next {
  from {
    border-radius: 0px;
    transform: translateZ(0px) rotateY(0deg);
  }
  to {
    border-radius: 30px;
    transform: translateZ(-100vmax) rotateY(180deg);
  }
}
@keyframes f7-flip-current-to-prev {
  from {
    border-radius: 0px;
    transform: translateZ(0px) rotateY(0deg);
  }
  to {
    border-radius: 30px;
    transform: translateZ(-100vmax) rotateY(-180deg);
  }
}
@keyframes f7-flip-prev-to-current {
  from {
    border-radius: 30px;
    transform: translateZ(-100vmax) rotateY(-180deg);
  }
  to {
    border-radius: 0px;
    transform: translateZ(0px) rotateY(0deg);
  }
}
.router-transition-f7-parallax-forward .page-next {
  animation: f7-parallax-next-to-current 500ms forwards;
}
.router-transition-f7-parallax-forward .page-current {
  animation: f7-parallax-current-to-prev 500ms forwards;
}
.router-transition-f7-parallax-backward .page-current {
  animation: f7-parallax-current-to-next 500ms forwards;
}
.router-transition-f7-parallax-backward .page-previous {
  animation: f7-parallax-prev-to-current 500ms forwards;
}
@keyframes f7-parallax-next-to-current {
  from {
    transform: translateX(100%);
  }
  to {
    transform: translateX(0%);
  }
}
@keyframes f7-parallax-current-to-next {
  from {
    transform: translateX(0%);
  }
  to {
    transform: translateX(100%);
  }
}
@keyframes f7-parallax-current-to-prev {
  from {
    transform: translateX(0%);
  }
  to {
    transform: translateX(-20%);
  }
}
@keyframes f7-parallax-prev-to-current {
  from {
    transform: translateX(-20%);
  }
  to {
    transform: translateX(0%);
  }
}
.router-transition-f7-push-forward .page-next {
  animation: f7-push-next-to-current 500ms forwards;
}
.router-transition-f7-push-forward .page-current {
  animation: f7-push-current-to-prev 500ms forwards;
}
.router-transition-f7-push-backward .page-current {
  animation: f7-push-current-to-next 500ms forwards;
}
.router-transition-f7-push-backward .page-previous {
  animation: f7-push-prev-to-current 500ms forwards;
}
@keyframes f7-push-next-to-current {
  from {
    transform: translateX(100%);
  }
  to {
    transform: translateX(0%);
  }
}
@keyframes f7-push-current-to-next {
  from {
    transform: translateX(0%);
  }
  to {
    transform: translateX(100%);
  }
}
@keyframes f7-push-current-to-prev {
  from {
    transform: translateX(0%);
  }
  to {
    transform: translateX(-100%);
  }
}
@keyframes f7-push-prev-to-current {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0%);
  }
}
/* === Link === */
:root {
  --f7-link-highlight-black: rgba(0, 0, 0, 0.1);
  --f7-link-highlight-white: rgba(255, 255, 255, 0.15);
  --f7-link-highlight-color: var(--f7-link-highlight-black);
}
.theme-dark {
  --f7-link-highlight-color: var(--f7-link-highlight-white);
}
.link,
.tab-link {
  display: inline-flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  position: relative;
  box-sizing: border-box;
  z-index: 1;
}
.link i + span,
.link i + i,
.link span + i,
.link span + span {
  margin-left: 4px;
}
.ios .link {
  transition: opacity 300ms;
}
.ios .link.active-state {
  opacity: 0.3;
  transition-duration: 0ms;
}
.aurora .link {
  transition: opacity 300ms;
}
.aurora .link.active-state {
  opacity: 0.3;
  transition-duration: 0ms;
}
/* === Navbar === */
:root {
  /*
  --f7-navbar-bg-color: var(--f7-bars-bg-color);
  --f7-navbar-bg-color-rgb: var(--f7-bars-bg-color-rgb);
  --f7-navbar-bg-image: var(--f7-bars-bg-image);
  --f7-navbar-border-color: var(--f7-bars-border-color);
  --f7-navbar-link-color: var(--f7-bars-link-color);
  --f7-navbar-text-color: var(--f7-bars-text-color);
  */
  --f7-navbar-hide-show-transition-duration: 400ms;
  --f7-navbar-title-line-height: 1.2;
  --f7-navbar-title-font-size: inherit;
  --f7-navbar-subtitle-text-align: inherit;
  --f7-navbar-large-title-line-height: 1.2;
  --f7-navbar-large-title-text-color: inherit;
  --f7-navbar-large-title-padding-left: 16px;
  --f7-navbar-large-title-padding-right: 16px;
}
.ios {
  --f7-navbar-height: 44px;
  --f7-navbar-tablet-height: 44px;
  --f7-navbar-font-size: 17px;
  --f7-navbar-inner-padding-left: 8px;
  --f7-navbar-inner-padding-right: 8px;
  --f7-navbar-title-font-weight: 600;
  --f7-navbar-title-margin-left: 0;
  --f7-navbar-title-margin-right: 0;
  --f7-navbar-title-text-align: center;
  --f7-navbar-subtitle-font-size: 10px;
  --f7-navbar-subtitle-line-height: 1;
  --f7-navbar-shadow-image: none;
  --f7-navbar-large-title-height: 52px;
  --f7-navbar-large-title-font-size: 34px;
  --f7-navbar-large-title-font-weight: 700;
  --f7-navbar-large-title-letter-spacing: -0.03em;
  --f7-navbar-large-title-padding-vertical: 6px;
  /*
  --f7-navbar-link-height: var(--f7-navbar-height);
  --f7-navbar-link-line-height: var(--f7-navbar-height);
  */
  --f7-navbar-subtitle-text-color: rgba(0, 0, 0, 0.55);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-navbar-subtitle-text-color: rgba(255, 255, 255, 0.55);
}
.md {
  --f7-navbar-height: 56px;
  --f7-navbar-tablet-height: 64px;
  --f7-navbar-font-size: 20px;
  --f7-navbar-inner-padding-left: 0px;
  --f7-navbar-inner-padding-right: 0px;
  --f7-navbar-title-font-weight: 500;
  --f7-navbar-title-margin-left: 16px;
  --f7-navbar-title-margin-right: 16px;
  --f7-navbar-title-text-align: left;
  --f7-navbar-subtitle-font-size: 14px;
  --f7-navbar-subtitle-line-height: 1.2;
  --f7-navbar-shadow-image: var(--f7-bars-shadow-bottom-image);
  --f7-navbar-large-title-font-size: 34px;
  --f7-navbar-large-title-height: 56px;
  --f7-navbar-large-title-font-weight: 500;
  --f7-navbar-large-title-letter-spacing: 0;
  --f7-navbar-large-title-padding-vertical: 8px;
  /*
  --f7-navbar-link-height: var(--f7-navbar-height);
  --f7-navbar-link-line-height: var(--f7-navbar-height);
  */
  --f7-navbar-subtitle-text-color: rgba(0, 0, 0, 0.85);
}
.md .theme-dark,
.md.theme-dark {
  --f7-navbar-subtitle-text-color: rgba(255, 255, 255, 0.85);
}
.aurora {
  --f7-navbar-height: 38px;
  --f7-navbar-tablet-height: 38px;
  --f7-navbar-font-size: 14px;
  --f7-navbar-inner-padding-left: 16px;
  --f7-navbar-inner-padding-right: 16px;
  --f7-navbar-title-font-weight: 600;
  --f7-navbar-title-margin-left: 0;
  --f7-navbar-title-margin-right: 0;
  --f7-navbar-title-text-align: center;
  --f7-navbar-subtitle-font-size: 12px;
  --f7-navbar-subtitle-line-height: 1;
  --f7-navbar-shadow-image: none;
  --f7-navbar-large-title-height: 38px;
  --f7-navbar-large-title-font-size: 26px;
  --f7-navbar-large-title-font-weight: bold;
  --f7-navbar-large-title-letter-spacing: -0.03em;
  --f7-navbar-large-title-padding-vertical: 4px;
  --f7-navbar-link-height: auto;
  --f7-navbar-link-line-height: inherit;
  --f7-navbar-subtitle-text-color: rgba(0, 0, 0, 0.6);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-navbar-subtitle-text-color: rgba(255, 255, 255, 0.5);
}
.navbars,
.navbar {
  z-index: 500;
  left: 0;
  top: 0;
  width: 100%;
}
.navbars {
  position: absolute;
}
.navbars .navbar {
  z-index: auto;
}
.navbar {
  --f7-navbar-large-collapse-progress: 0;
  position: relative;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  box-sizing: border-box;
  margin: 0;
  height: calc(var(--f7-navbar-height) + var(--f7-safe-area-top));
  color: var(--f7-navbar-text-color, var(--f7-bars-text-color));
  font-size: var(--f7-navbar-font-size);
}
.navbar.stacked {
  display: none;
}
.navbar b {
  font-weight: 500;
}
.navbar a {
  color: var(--f7-navbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.navbar a.link {
  display: flex;
  justify-content: flex-start;
  line-height: var(--f7-navbar-link-line-height, var(--f7-navbar-height));
  height: var(--f7-navbar-link-height, var(--f7-navbar-height));
}
.navbar .title,
.navbar .left,
.navbar .right {
  position: relative;
  z-index: 10;
}
.navbar .title {
  position: relative;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
  flex-shrink: 10;
  font-weight: var(--f7-navbar-title-font-weight);
  display: inline-block;
  line-height: var(--f7-navbar-title-line-height);
  text-align: var(--f7-navbar-title-text-align);
  font-size: var(--f7-navbar-title-font-size);
  margin-left: var(--f7-navbar-title-margin-left);
  margin-right: var(--f7-navbar-title-margin-left);
}
.navbar .subtitle {
  display: block;
  color: var(--f7-navbar-subtitle-text-color);
  font-weight: normal;
  font-size: var(--f7-navbar-subtitle-font-size);
  line-height: var(--f7-navbar-subtitle-line-height);
  text-align: var(--f7-navbar-subtitle-text-align);
}
.navbar .left,
.navbar .right {
  flex-shrink: 0;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
.navbar .right:first-child {
  position: absolute;
  height: 100%;
}
.navbar.no-hairline .navbar-bg:after,
.navbar.no-border .navbar-bg:after,
.navbar .no-hairline .navbar-bg:after,
.navbar .no-border .navbar-bg:after {
  display: none !important;
}
.navbar.no-hairline .title-large:after,
.navbar.no-border .title-large:after,
.navbar .no-hairline .title-large:after,
.navbar .no-border .title-large:after {
  display: none !important;
}
.navbar.no-shadow .navbar-bg:before,
.navbar .no-shadow .navbar-bg:before {
  display: none !important;
}
.navbar.navbar-hidden .navbar-bg:before,
.navbar-hidden .navbar .navbar-bg:before {
  opacity: 0 !important;
}
.navbar-bg {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  background: var(--f7-navbar-bg-color);
  background-image: var(--f7-navbar-bg-image, var(--f7-bars-bg-image));
  background-color: var(--f7-navbar-bg-color, var(--f7-bars-bg-color));
  transition-property: transform;
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .navbar-bg {
    background-color: rgba(var(--f7-navbar-bg-color-rgb, var(--f7-bars-bg-color-rgb)), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.navbar-bg:after,
.navbar-bg:before {
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.navbar-bg:after {
  content: '';
  position: absolute;
  background-color: var(--f7-navbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.navbar-bg:before {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  top: 100%;
  bottom: auto;
  height: 8px;
  pointer-events: none;
  background: var(--f7-navbar-shadow-image);
}
.navbar-bg:after {
  z-index: 1;
}
@media (min-width: 768px) and (min-height: 600px) {
  :root {
    --f7-navbar-height: var(--f7-navbar-tablet-height);
  }
}
.navbar-transitioning,
.navbar-transitioning .left,
.navbar-transitioning .title,
.navbar-transitioning .right,
.navbar-transitioning .title-large-text,
.navbar-transitioning .navbar-bg,
.navbar-transitioning .subnavbar,
.navbar-transitioning .navbar-bg:before {
  transition-duration: var(--f7-navbar-hide-show-transition-duration);
}
.navbar-page-transitioning {
  transition-duration: var(--f7-page-swipeback-transition-duration) !important;
}
.navbar-page-transitioning .title-large-text,
.navbar-page-transitioning .navbar-bg {
  transition-duration: var(--f7-page-swipeback-transition-duration) !important;
}
.navbar-hidden {
  transform: translate3d(0, calc(-1 * var(--f7-navbar-height)), 0);
}
.navbar-hidden .navbar-inner {
  pointer-events: none;
}
.navbar-hidden .navbar-inner > .left,
.navbar-hidden .navbar-inner > .title,
.navbar-hidden .navbar-inner > .right {
  opacity: 0 !important;
}
.navbar-hidden-statusbar {
  transform: translate3d(0, calc(-1 * var(--f7-navbar-height) - var(--f7-safe-area-top)), 0);
}
.navbar-large-hidden .navbar-large {
  --f7-navbar-large-collapse-progress: 1;
}
.navbar-inner {
  position: absolute;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  box-sizing: border-box;
  padding: var(--f7-safe-area-top) calc(var(--f7-navbar-inner-padding-right) + var(--f7-safe-area-right)) 0 calc(var(--f7-navbar-inner-padding-left) + var(--f7-safe-area-left));
  transform: translate3d(0, 0, 0);
}
.views > .navbar,
.view > .navbar,
.page > .navbar,
.navbars > .navbar {
  position: absolute;
}
.navbar-large .navbar-bg,
.ios .router-navbar-transition-to-large .navbar-bg,
.ios .router-navbar-transition-from-large .navbar-bg,
.navbar-bg.ios-swipeback-navbar-bg-large,
.navbar-large-transparent .navbar-bg.ios-swipeback-navbar-bg-large {
  height: calc(100% + var(--f7-navbar-large-title-height));
  transform: translate3d(0px, calc(-1 * var(--f7-navbar-large-collapse-progress) * var(--f7-navbar-large-title-height)), 0);
}
.navbar-large-transparent .navbar-bg {
  opacity: var(--f7-navbar-large-collapse-progress);
  height: 100%;
  transform: none;
}
.ios .navbar:not(.navbar-large) .navbar-bg {
  --f7-navbar-large-collapse-progress: 1;
}
.navbar-large .title {
  opacity: var(--f7-navbar-large-collapse-progress);
}
.navbar-large-collapsed {
  --f7-navbar-large-collapse-progress: 1;
}
.navbar-large-collapsed .title-large {
  pointer-events: none;
}
.navbar .title-large {
  box-sizing: border-box;
  position: absolute;
  left: 0;
  right: 0;
  top: 100%;
  display: flex;
  align-items: flex-end;
  white-space: nowrap;
  overflow: hidden;
  height: var(--f7-navbar-large-title-height);
  z-index: 5;
}
.navbar .title-large-text {
  text-overflow: ellipsis;
  white-space: nowrap;
  color: var(--f7-navbar-large-title-text-color);
  letter-spacing: var(--f7-navbar-large-title-letter-spacing);
  font-size: var(--f7-navbar-large-title-font-size);
  font-weight: var(--f7-navbar-large-title-font-weight);
  line-height: var(--f7-navbar-large-title-line-height);
  padding-left: calc(var(--f7-navbar-large-title-padding-left) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-navbar-large-title-padding-right) + var(--f7-safe-area-right));
  padding-top: var(--f7-navbar-large-title-padding-vertical);
  padding-bottom: var(--f7-navbar-large-title-padding-vertical);
  box-sizing: border-box;
  overflow: hidden;
  width: 100%;
  transform: translate3d(0px, calc(-1 * var(--f7-navbar-large-collapse-progress) * var(--f7-navbar-large-title-height)), 0);
  transform-origin: calc(var(--f7-navbar-large-title-padding-left) + var(--f7-safe-area-left)) center;
}
.navbar-no-title-large-transition .title-large-text {
  transition-duration: 0ms;
}
.navbar ~ *,
.navbars ~ * {
  --f7-page-navbar-offset: calc(var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbar ~ * .page-with-navbar-large,
.navbar ~ .page-with-navbar-large,
.navbars ~ * .page-with-navbar-large,
.navbars ~ .page-with-navbar-large,
.page-with-navbar-large .navbar ~ * {
  --f7-page-navbar-offset: calc(var(--f7-navbar-height) + var(--f7-navbar-large-title-height) + var(--f7-safe-area-top));
}
.page.no-navbar,
.page.no-navbar .navbar ~ * {
  --f7-page-navbar-offset: var(--f7-safe-area-top);
}
.ios {
  --f7-navbarLeftTextOffset: calc(4px + 12px + var(--f7-navbar-inner-padding-left));
  --f7-navbarTitleLargeOffset: var(--f7-navbar-large-title-padding-left);
  --f7-navbar-large-transparent-bg-center: translateX(0);
  --f7-navbar-large-bg-center-top: translateX(0) translateY(calc(-1 * var(--f7-navbar-large-title-height)));
  --f7-navbar-large-bg-center-bottom: translateX(0) translateY(0);
  --f7-navbar-large-transparent-bg-left: translateX(-100%);
  --f7-navbar-large-bg-left-top: translateX(-100%) translateY(calc(-1 * var(--f7-navbar-large-title-height)));
  --f7-navbar-large-bg-left-bottom: translateX(-100%) translateY(0);
  --f7-navbar-large-bg-right-top: translateX(100%) translateY(calc(-1 * var(--f7-navbar-large-title-height)));
  --f7-navbar-large-bg-right-bottom: translateX(100%) translateY(0);
}
.ios .navbar a.icon-only {
  width: 44px;
  margin: 0;
  justify-content: center;
}
.ios .navbar .left a + a,
.ios .navbar .right a + a {
  margin-left: 16px;
}
.ios .navbar b {
  font-weight: 600;
}
.ios .navbar .left {
  margin-right: 10px;
}
.ios .navbar .right {
  margin-left: 10px;
}
.ios .navbar .right:first-child {
  right: calc(8px + var(--f7-safe-area-right));
}
.ios .navbar-inner {
  justify-content: space-between;
}
.ios .navbar-inner-left-title {
  justify-content: flex-start;
}
.ios .navbar-inner-left-title .right {
  margin-left: auto;
}
.ios .navbar-inner-left-title .title {
  text-align: left;
  margin-right: 10px;
}
.ios .view-master-detail .navbar-previous:not(.navbar-master) .left,
.ios .view:not(.view-master-detail) .navbar-previous .left,
.ios .navbar-next .left,
.ios .view-master-detail .navbar-previous:not(.navbar-master) .title,
.ios .view:not(.view-master-detail) .navbar-previous .title,
.ios .navbar-next .title,
.ios .view-master-detail .navbar-previous:not(.navbar-master) .right,
.ios .view:not(.view-master-detail) .navbar-previous .right,
.ios .navbar-next .right,
.ios .view-master-detail .navbar-previous:not(.navbar-master) .subnavbar,
.ios .view:not(.view-master-detail) .navbar-previous .subnavbar,
.ios .navbar-next .subnavbar,
.ios .view-master-detail .navbar-previous:not(.navbar-master) .fading,
.ios .view:not(.view-master-detail) .navbar-previous .fading,
.ios .navbar-next .fading {
  opacity: 0;
}
.ios .view-master-detail .navbar-previous:not(.navbar-master),
.ios .view:not(.view-master-detail) .navbar-previous {
  pointer-events: none;
}
.ios .view-master-detail .navbar-previous:not(.navbar-master) .title-large,
.ios .view:not(.view-master-detail) .navbar-previous .title-large {
  opacity: 0;
  transition-duration: 0ms;
}
.ios .view-master-detail .navbar-previous:not(.navbar-master) .title-large .title-large-text,
.ios .view:not(.view-master-detail) .navbar-previous .title-large .title-large-text {
  transform: scale(0.5);
  transition-duration: 0ms;
}
.ios .view-master-detail .navbar-previous:not(.navbar-master) .subnavbar.sliding,
.ios .view:not(.view-master-detail) .navbar-previous .subnavbar.sliding,
.ios .view-master-detail .navbar-previous:not(.navbar-master) .sliding .subnavbar,
.ios .view:not(.view-master-detail) .navbar-previous .sliding .subnavbar {
  opacity: 1;
  transform: translate3d(-100%, 0, 0);
}
.ios .view:not(.view-master-detail) .navbar-previous .navbar-bg,
.ios .view-master-detail .navbar-previous:not(.navbar-master) .navbar-bg {
  transform: translateX(-100%);
}
.ios .navbar-next {
  pointer-events: none;
}
.ios .navbar-next .navbar-bg {
  transform: translateX(100%);
}
.ios .navbar-next .title-large .title-large-text {
  transition-duration: 0ms;
  transform: translateX(100%) translateY(calc(-1 * var(--f7-navbar-large-title-height)));
}
.ios .navbar-next .subnavbar.sliding,
.ios .navbar-next .sliding .subnavbar {
  opacity: 1;
  transform: translate3d(100%, 0, 0);
}
.ios .router-transition .navbar,
.ios .router-transition .navbar-bg {
  transition-duration: var(--f7-page-transition-duration);
}
.ios .router-transition .navbar-bg {
  animation-duration: var(--f7-page-transition-duration);
  animation-fill-mode: forwards;
}
.ios .router-transition .title-large,
.ios .router-transition .title-large-text {
  transition-duration: 0ms;
}
.ios .router-transition .navbar-current .left,
.ios .router-transition .navbar-current .title,
.ios .router-transition .navbar-current .right,
.ios .router-transition .navbar-current .subnavbar {
  animation: ios-navbar-element-fade-out var(--f7-page-transition-duration) forwards;
}
.ios .router-transition .navbar-current .sliding.left,
.ios .router-transition .navbar-current .sliding.left .icon + span,
.ios .router-transition .navbar-current .sliding.title,
.ios .router-transition .navbar-current .sliding.right,
.ios .router-transition .navbar-current .sliding .left,
.ios .router-transition .navbar-current .sliding .left .icon + span,
.ios .router-transition .navbar-current .sliding .title,
.ios .router-transition .navbar-current .sliding .right {
  transition-duration: var(--f7-page-transition-duration);
  opacity: 0 !important;
  animation: none;
}
.ios .router-transition .navbar-current .sliding .subnavbar,
.ios .router-transition .navbar-current .sliding.subnavbar {
  transition-duration: var(--f7-page-transition-duration);
  animation: none;
  opacity: 1;
}
.ios .router-transition-forward .navbar-next .left,
.ios .router-transition-backward .navbar-previous .left,
.ios .router-transition-forward .navbar-next .title,
.ios .router-transition-backward .navbar-previous .title,
.ios .router-transition-forward .navbar-next .right,
.ios .router-transition-backward .navbar-previous .right,
.ios .router-transition-forward .navbar-next .subnavbar,
.ios .router-transition-backward .navbar-previous .subnavbar {
  animation: ios-navbar-element-fade-in var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .navbar-next .sliding.left,
.ios .router-transition-backward .navbar-previous .sliding.left,
.ios .router-transition-forward .navbar-next .sliding.left .icon + span,
.ios .router-transition-backward .navbar-previous .sliding.left .icon + span,
.ios .router-transition-forward .navbar-next .sliding.title,
.ios .router-transition-backward .navbar-previous .sliding.title,
.ios .router-transition-forward .navbar-next .sliding.right,
.ios .router-transition-backward .navbar-previous .sliding.right,
.ios .router-transition-forward .navbar-next .sliding .left,
.ios .router-transition-backward .navbar-previous .sliding .left,
.ios .router-transition-forward .navbar-next .sliding .left .icon + span,
.ios .router-transition-backward .navbar-previous .sliding .left .icon + span,
.ios .router-transition-forward .navbar-next .sliding .title,
.ios .router-transition-backward .navbar-previous .sliding .title,
.ios .router-transition-forward .navbar-next .sliding .right,
.ios .router-transition-backward .navbar-previous .sliding .right,
.ios .router-transition-forward .navbar-next .sliding .subnavbar,
.ios .router-transition-backward .navbar-previous .sliding .subnavbar {
  transition-duration: var(--f7-page-transition-duration);
  animation: none;
  transform: translate3d(0, 0, 0) !important;
  opacity: 1 !important;
}
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled-no-transition .left,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled .left,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled-no-transition .title,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled .title,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled-no-transition .right,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled .right,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled-no-transition .subnavbar,
.ios .router-transition-backward .navbar-previous.with-searchbar-expandable-enabled .subnavbar {
  animation: none;
}
.ios .router-transition-forward .navbar-current.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large,
.ios .router-transition-forward .navbar-current.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .title-large {
  overflow: visible;
}
.ios .router-transition-forward .navbar-current.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large .title-large-text,
.ios .router-transition-forward .navbar-current.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .title-large .title-large-text {
  animation: ios-navbar-large-title-text-slide-up var(--f7-page-transition-duration) forwards, ios-navbar-large-title-text-fade-out var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .navbar-next.router-navbar-transition-from-large .left .back span {
  animation: ios-navbar-back-text-next-to-current var(--f7-page-transition-duration) forwards;
  transition: none;
  transform-origin: left center;
}
.ios .router-transition-forward .navbar-next.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large {
  overflow: visible;
}
.ios .router-transition-forward .navbar-next.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large .title-large-text {
  animation: ios-navbar-large-title-text-slide-left var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .navbar-next.router-navbar-transition-to-large:not(.router-navbar-transition-from-large) .title-large .title-large-text {
  animation: ios-navbar-large-title-text-slide-left var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-forward .navbar-next.navbar-large:not(.navbar-large-collapsed) .title,
.ios .router-transition-forward .navbar-current.navbar-large:not(.navbar-large-collapsed) .title {
  animation: none;
  opacity: 0 !important;
  transition-duration: 0;
}
.ios .router-transition-backward .navbar-current.router-navbar-transition-to-large .left .back span {
  animation: ios-navbar-back-text-current-to-previous var(--f7-page-transition-duration) forwards;
  transition: none;
  transform-origin: left center;
}
.ios .router-transition-backward .navbar-current.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large {
  overflow: visible;
}
.ios .router-transition-backward .navbar-current.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large .title-large-text {
  animation: ios-navbar-large-title-text-slide-right var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .navbar-current.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .title-large .title-large-text {
  animation: ios-navbar-large-title-text-slide-right var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .navbar-current.router-navbar-transition-to-large:not(.router-navbar-transition-from-large) .title-large {
  opacity: 0;
}
.ios .router-transition-backward .navbar-previous.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large,
.ios .router-transition-backward .navbar-previous.router-navbar-transition-to-large:not(.router-navbar-transition-from-large) .title-large {
  overflow: visible;
  opacity: 1;
}
.ios .router-transition-backward .navbar-previous.router-navbar-transition-from-large.router-navbar-transition-to-large .title-large .title-large-text,
.ios .router-transition-backward .navbar-previous.router-navbar-transition-to-large:not(.router-navbar-transition-from-large) .title-large .title-large-text {
  animation: ios-navbar-large-title-text-slide-down var(--f7-page-transition-duration) forwards, ios-navbar-large-title-text-fade-in var(--f7-page-transition-duration) forwards;
}
.ios .router-transition-backward .navbar-current.navbar-large:not(.navbar-large-collapsed) .title,
.ios .router-transition-backward .navbar-previous.navbar-large:not(.navbar-large-collapsed) .title {
  animation: none;
  opacity: 0 !important;
  transition-duration: 0;
}
.ios .router-transition-forward .navbar-current .navbar-bg {
  animation-name: ios-navbar-bg-from-cb-to-lb;
}
.ios .router-transition-forward .navbar-current.router-navbar-transition-from-large.router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-cb-to-lb;
}
.ios .router-transition-forward .navbar-current.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .navbar-bg {
  animation-name: ios-navbar-bg-from-cb-to-lt;
}
.ios .router-transition-forward .navbar-current:not(.router-navbar-transition-from-large).router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-ct-to-lb;
}
.ios .router-transition-forward .navbar-current.navbar-large-collapsed:not(.router-navbar-transition-to-large) .navbar-bg {
  animation-name: ios-navbar-bg-from-ct-to-lt;
}
.ios .router-transition-forward .navbar-current.navbar-large-collapsed.navbar-large-transparent:not(.router-navbar-transition-to-large) .navbar-bg {
  animation-name: ios-navbar-transparent-bg-from-c-to-l;
}
.ios .router-transition-forward .navbar-next .navbar-bg {
  animation-name: ios-navbar-bg-from-rb-to-cb;
}
.ios .router-transition-forward .navbar-next.router-navbar-transition-from-large.router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-rb-to-cb;
}
.ios .router-transition-forward .navbar-next.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .navbar-bg {
  animation-name: ios-navbar-bg-from-rb-to-ct;
}
.ios .router-transition-forward .navbar-next:not(.router-navbar-transition-from-large).router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-rt-to-cb;
}
.ios .router-transition-backward .navbar-current .navbar-bg {
  animation-name: ios-navbar-bg-from-cb-to-rb;
}
.ios .router-transition-backward .navbar-current:not(.router-navbar-transition-from-large).router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-ct-to-rb;
}
.ios .router-transition-backward .navbar-current.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .navbar-bg {
  animation-name: ios-navbar-bg-from-cb-to-rt;
}
.ios .router-transition-backward .navbar-current.navbar-large-collapsed .navbar-bg {
  animation-name: ios-navbar-bg-from-ct-to-rt;
}
.ios .router-transition-backward .navbar-current.navbar-large-collapsed.navbar-large-transparent .navbar-bg {
  animation-name: ios-navbar-bg-from-cb-to-rb;
}
.ios .router-transition-backward .navbar-current.navbar-large-collapsed.router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-ct-to-rb;
}
.ios .router-transition-backward .navbar-previous .navbar-bg {
  animation-name: ios-navbar-bg-from-lb-to-cb;
}
.ios .router-transition-backward .navbar-previous:not(.router-navbar-transition-from-large).router-navbar-transition-to-large .navbar-bg {
  animation-name: ios-navbar-bg-from-lt-to-cb;
}
.ios .router-transition-backward .navbar-previous.router-navbar-transition-from-large:not(.router-navbar-transition-to-large) .navbar-bg {
  animation-name: ios-navbar-bg-from-lb-to-ct;
}
.ios .router-transition-backward .navbar-previous.navbar-large-collapsed .navbar-bg {
  animation-name: ios-navbar-bg-from-lt-to-ct;
}
.ios .router-transition-backward .navbar-previous.navbar-large-collapsed.navbar-large-transparent .navbar-bg {
  animation-name: ios-navbar-transparent-bg-from-l-to-c;
}
.ios .router-transition-backward .navbar-previous.navbar-large-collapsed.navbar-large-transparent.router-navbar-transition-from-large .navbar-bg {
  animation-name: ios-navbar-bg-from-lb-to-ct;
}
.view-master-detail .navbars {
  z-index: auto;
}
.view-master-detail .page-master {
  z-index: 525;
}
.view-master-detail .navbar-master .navbar-inner,
.view-master-detail .navbar-master .navbar-bg {
  z-index: 550;
}
.view-master-detail .navbar-master-detail .navbar-inner,
.view-master-detail .navbar-master-detail .navbar-bg {
  z-index: 500;
}
.view-master-detail .navbar-master.navbar-previous {
  pointer-events: auto;
}
.view-master-detail .navbar-master.navbar-previous .left,
.view-master-detail .navbar-master.navbar-previous:not(.navbar-large) .title,
.view-master-detail .navbar-master.navbar-previous .right,
.view-master-detail .navbar-master.navbar-previous .subnavbar {
  opacity: 1;
}
.view-master-detail.router-transition .navbar-master .left,
.view-master-detail.router-transition .navbar-master .left .icon + span,
.view-master-detail.router-transition .navbar-master:not(.navbar-large) .title,
.view-master-detail.router-transition .navbar-master .right,
.view-master-detail.router-transition .navbar-master .subnavbar,
.view-master-detail.router-transition .navbar-master .fading {
  opacity: 1 !important;
  transition-duration: 0ms;
  transform: none !important;
  animation: none !important;
}
.view-master-detail.router-transition .navbar-master .navbar-bg {
  transition-duration: 0ms;
  animation: none !important;
}
.view-master-detail.router-transition .navbar-master.navbar-large .title {
  opacity: calc(-1 + 2 * var(--f7-navbar-large-collapse-progress)) !important;
  transition-duration: 0ms;
  transform: none !important;
  animation: none !important;
}
.view-master-detail.router-transition .navbar-master.navbar-large .title-large,
.view-master-detail.router-transition .navbar-master.navbar-large .title-large-text {
  transition-duration: 0ms;
  animation: none !important;
}
.view-master-detail.router-transition .navbar-master.navbar-large-transparent .navbar-bg {
  height: 100% !important;
  opacity: var(--f7-navbar-large-collapse-progress) !important;
}
@keyframes ios-navbar-element-fade-in {
  0% {
    opacity: 0;
  }
  25% {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes ios-navbar-element-fade-out {
  from {
    opacity: 1;
  }
  75% {
    opacity: 0;
  }
  to {
    opacity: 0;
  }
}
@keyframes ios-navbar-large-title-text-slide-up {
  0% {
    transform: translateX(0px) translateY(0%) scale(1);
  }
  100% {
    transform: translateX(calc(var(--f7-navbarLeftTextOffset) - var(--f7-navbarTitleLargeOffset))) translateY(calc(-1 * var(--f7-navbar-large-title-height) + var(--f7-navbar-large-title-padding-vertical))) scale(0.5);
  }
}
@keyframes ios-navbar-large-title-text-slide-down {
  0% {
    transform: translateX(calc(var(--f7-navbarLeftTextOffset) - var(--f7-navbarTitleLargeOffset))) translateY(calc(-1 * var(--f7-navbar-large-title-height) + var(--f7-navbar-large-title-padding-vertical) / 2)) scale(0.5);
  }
  100% {
    transform: translateX(0px) translateY(0%) scale(1);
  }
}
@keyframes ios-navbar-large-title-text-slide-left {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(0%);
  }
}
@keyframes ios-navbar-large-title-text-slide-right {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(100%);
  }
}
@keyframes ios-navbar-large-title-text-fade-out {
  0% {
    opacity: 1;
  }
  80% {
    opacity: 0;
  }
  100% {
    opacity: 0;
  }
}
@keyframes ios-navbar-large-title-text-fade-in {
  0% {
    opacity: 0;
  }
  20% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
@keyframes ios-navbar-back-text-current-to-previous {
  0% {
    opacity: 1;
    transform: translateY(0px) translateX(0px) scale(1);
  }
  80% {
    opacity: 0;
  }
  100% {
    opacity: 0;
    transform: translateX(calc(var(--f7-navbarTitleLargeOffset) - var(--f7-navbarLeftTextOffset))) translateY(calc(1 * var(--f7-navbar-large-title-height) - var(--f7-navbar-large-title-padding-vertical) / 2)) scale(2);
  }
}
@keyframes ios-navbar-back-text-next-to-current {
  0% {
    opacity: 0;
    transform: translateX(calc(var(--f7-navbarTitleLargeOffset) - var(--f7-navbarLeftTextOffset))) translateY(calc(1 * var(--f7-navbar-large-title-height) + var(--f7-navbar-large-title-padding-vertical) / 2)) scale(2);
  }
  20% {
    opacity: 0;
  }
  100% {
    opacity: 1;
    transform: translateX(0px) translateY(0px) scale(1);
  }
}
@keyframes ios-navbar-bg-from-cb-to-lb {
  from {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-left-bottom);
  }
}
@keyframes ios-navbar-bg-from-cb-to-lt {
  from {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-left-top);
  }
}
@keyframes ios-navbar-bg-from-ct-to-lb {
  from {
    transform: var(--f7-navbar-large-bg-center-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-left-bottom);
  }
}
@keyframes ios-navbar-bg-from-ct-to-lt {
  from {
    transform: var(--f7-navbar-large-bg-center-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-left-top);
  }
}
@keyframes ios-navbar-bg-from-rb-to-cb {
  from {
    transform: var(--f7-navbar-large-bg-right-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
}
@keyframes ios-navbar-bg-from-rb-to-ct {
  from {
    transform: var(--f7-navbar-large-bg-right-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-top);
  }
}
@keyframes ios-navbar-bg-from-rt-to-cb {
  from {
    transform: var(--f7-navbar-large-bg-right-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
}
@keyframes ios-navbar-bg-from-cb-to-rb {
  from {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-right-bottom);
  }
}
@keyframes ios-navbar-bg-from-ct-to-rb {
  from {
    transform: var(--f7-navbar-large-bg-center-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-right-bottom);
  }
}
@keyframes ios-navbar-bg-from-cb-to-rt {
  from {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-right-top);
  }
}
@keyframes ios-navbar-bg-from-ct-to-rt {
  from {
    transform: var(--f7-navbar-large-bg-center-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-right-top);
  }
}
@keyframes ios-navbar-bg-from-lb-to-cb {
  from {
    transform: var(--f7-navbar-large-bg-left-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
}
@keyframes ios-navbar-bg-from-lt-to-cb {
  from {
    transform: var(--f7-navbar-large-bg-left-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-bottom);
  }
}
@keyframes ios-navbar-bg-from-lb-to-ct {
  from {
    transform: var(--f7-navbar-large-bg-left-bottom);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-top);
  }
}
@keyframes ios-navbar-bg-from-lt-to-ct {
  from {
    transform: var(--f7-navbar-large-bg-left-top);
  }
  to {
    transform: var(--f7-navbar-large-bg-center-top);
  }
}
@keyframes ios-navbar-transparent-bg-from-l-to-c {
  from {
    transform: var(--f7-navbar-large-transparent-bg-left);
  }
  to {
    transform: var(--f7-navbar-large-transparent-bg-center);
  }
}
@keyframes ios-navbar-transparent-bg-from-c-to-l {
  from {
    transform: var(--f7-navbar-large-transparent-bg-center);
  }
  to {
    transform: var(--f7-navbar-large-transparent-bg-left);
  }
}
.md .navbar a.link {
  padding: 0 16px;
  min-width: 48px;
}
.md .navbar a.link:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .navbar a.link.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .navbar a.icon-only {
  min-width: 0;
  flex-shrink: 0;
  width: 56px;
}
.md .navbar .right {
  margin-left: auto;
}
.md .navbar .right:first-child {
  right: var(--f7-safe-area-right);
}
.md .navbar-inner {
  justify-content: flex-start;
  overflow: hidden;
}
.md .navbar-large:not(.navbar-large-collapsed) .navbar-inner {
  overflow: visible;
}
.md .page.page-with-subnavbar .navbar-inner {
  overflow: visible;
}
.md .navbar-inner-centered-title {
  justify-content: space-between;
}
.md .navbar-inner-centered-title .right {
  margin-left: 0;
}
.md .navbar-inner-centered-title .title {
  text-align: center;
}
.aurora .navbar a.icon-only {
  margin: 0;
  justify-content: center;
}
.aurora .navbar .left a + a,
.aurora .navbar .right a + a {
  margin-left: 10px;
}
.aurora .navbar b {
  font-weight: bold;
}
.aurora .navbar .left {
  margin-right: 10px;
}
.aurora .navbar .right {
  margin-left: 10px;
}
.aurora .navbar .right:first-child {
  right: calc(16px + var(--f7-safe-area-right));
}
.aurora .navbar-inner {
  justify-content: space-between;
}
.aurora .navbar-inner-left-title {
  justify-content: flex-start;
}
.aurora .navbar-inner-left-title .right {
  margin-left: auto;
}
.aurora .navbar-inner-left-title .title {
  text-align: left;
  margin-right: 10px;
}
/* === Toolbar === */
:root {
  /*
  --f7-toolbar-bg-color: var(--f7-bars-bg-color);
  --f7-toolbar-bg-color-rgb: var(--f7-bars-bg-color-rgb);
  --f7-toolbar-bg-image: var(--f7-bars-bg-image);
  --f7-toolbar-border-color: var(--f7-bars-border-color);
  --f7-toolbar-link-color: var(--f7-bars-link-color);
  --f7-toolbar-text-color: var(--f7-bars-text-color);
  --f7-tabbar-link-active-color: var(--f7-theme-color);
  */
  --f7-tabbar-link-active-bg-color: transparent;
  --f7-tabbar-label-text-transform: none;
  --f7-toolbar-hide-show-transition-duration: 400ms;
}
.ios {
  --f7-toolbar-height: 44px;
  --f7-toolbar-font-size: 17px;
  --f7-toolbar-inner-padding-left: 8px;
  --f7-toolbar-inner-padding-right: 8px;
  /*
  --f7-toolbar-link-height: var(--f7-toolbar-height);
  --f7-toolbar-link-line-height: var(--f7-toolbar-height);
  */
  --f7-tabbar-labels-height: 50px;
  --f7-tabbar-labels-tablet-height: 50px;
  --f7-toolbar-top-shadow-image: none;
  --f7-toolbar-bottom-shadow-image: none;
  --f7-tabbar-icon-size: 28px;
  --f7-tabbar-link-text-transform: none;
  --f7-tabbar-link-font-weight: 400;
  --f7-tabbar-link-letter-spacing: 0;
  --f7-tabbar-label-font-size: 12px;
  --f7-tabbar-label-tablet-font-size: 14px;
  --f7-tabbar-label-font-weight: 500;
  --f7-tabbar-label-letter-spacing: 0.01;
  --f7-tabbar-link-inactive-color: rgba(0, 0, 0, 0.4);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-tabbar-link-inactive-color: rgba(255, 255, 255, 0.54);
}
.md {
  --f7-toolbar-height: 48px;
  --f7-toolbar-font-size: 14px;
  --f7-toolbar-inner-padding-left: 0px;
  --f7-toolbar-inner-padding-right: 0px;
  /*
  --f7-toolbar-link-height: var(--f7-toolbar-height);
  --f7-toolbar-link-line-height: var(--f7-toolbar-height);
  */
  --f7-tabbar-labels-height: 56px;
  --f7-tabbar-labels-tablet-height: 56px;
  /*
  --f7-tabbar-link-active-border-color: var(--f7-theme-color);
  */
  --f7-toolbar-top-shadow-image: var(--f7-bars-shadow-bottom-image);
  --f7-toolbar-bottom-shadow-image: var(--f7-bars-shadow-top-image);
  --f7-tabbar-icon-size: 24px;
  --f7-tabbar-link-text-transform: uppercase;
  --f7-tabbar-link-font-weight: 500;
  --f7-tabbar-link-letter-spacing: 0.03em;
  --f7-tabbar-label-font-size: 14px;
  --f7-tabbar-label-tablet-font-size: 14px;
  --f7-tabbar-label-font-weight: 400;
  --f7-tabbar-label-letter-spacing: 0;
  --f7-tabbar-link-inactive-color: rgba(0, 0, 0, 0.54);
}
.md .theme-dark,
.md.theme-dark {
  --f7-tabbar-link-inactive-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-toolbar-height: 38px;
  --f7-toolbar-font-size: 14px;
  --f7-toolbar-inner-padding-left: 16px;
  --f7-toolbar-inner-padding-right: 16px;
  --f7-toolbar-link-height: auto;
  --f7-toolbar-link-line-height: inherit;
  --f7-tabbar-labels-height: 44px;
  --f7-tabbar-labels-tablet-height: 44px;
  --f7-tabbar-link-inactive-bg-color: rgba(0, 0, 0, 0.2);
  --f7-toolbar-top-shadow-image: none;
  --f7-toolbar-bottom-shadow-image: none;
  --f7-tabbar-icon-size: 18px;
  --f7-tabbar-link-text-transform: none;
  --f7-tabbar-link-font-weight: 400;
  --f7-tabbar-link-letter-spacing: 0;
  --f7-tabbar-label-font-size: 12px;
  --f7-tabbar-label-tablet-font-size: 12px;
  --f7-tabbar-label-font-weight: 500;
  --f7-tabbar-label-letter-spacing: 0.01;
  --f7-tabbar-link-inactive-color: rgba(0, 0, 0, 0.5);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-tabbar-link-inactive-color: rgba(255, 255, 255, 0.5);
}
.toolbar {
  width: 100%;
  position: relative;
  margin: 0;
  transform: translate3d(0, 0, 0);
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  z-index: 600;
  box-sizing: border-box;
  left: 0;
  height: var(--f7-toolbar-height);
  background-image: var(--f7-toolbar-bg-image, var(--f7-bars-bg-image));
  background-color: var(--f7-toolbar-bg-color, var(--f7-bars-bg-color));
  color: var(--f7-toolbar-text-color, var(--f7-bars-text-color));
  font-size: var(--f7-toolbar-font-size);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .toolbar {
    background-color: rgba(var(--f7-toolbar-bg-color-rgb, var(--f7-bars-bg-color-rgb)), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.toolbar b {
  font-weight: 600;
}
.toolbar a {
  color: var(--f7-toolbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
  box-sizing: border-box;
  flex-shrink: 1;
  position: relative;
  white-space: nowrap;
  text-overflow: ellipsis;
}
.toolbar .link {
  display: flex;
  line-height: var(--f7-toolbar-link-line-height, var(--f7-toolbar-height));
  height: var(--f7-toolbar-link-height, var(--f7-toolbar-height));
}
.toolbar i.icon {
  display: block;
}
.toolbar:after,
.toolbar:before {
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.views > .toolbar,
.view > .toolbar,
.page > .toolbar {
  position: absolute;
}
.toolbar-top,
.ios .toolbar-top-ios,
.md .toolbar-top-md,
.aurora .toolbar-top-aurora {
  top: 0;
}
.toolbar-top .tab-link-highlight,
.ios .toolbar-top-ios .tab-link-highlight,
.md .toolbar-top-md .tab-link-highlight,
.aurora .toolbar-top-aurora .tab-link-highlight {
  bottom: 0;
}
.toolbar-top.no-hairline:after,
.ios .toolbar-top-ios.no-hairline:after,
.md .toolbar-top-md.no-hairline:after,
.aurora .toolbar-top-aurora.no-hairline:after,
.toolbar-top.no-border:after,
.ios .toolbar-top-ios.no-border:after,
.md .toolbar-top-md.no-border:after,
.aurora .toolbar-top-aurora.no-border:after {
  display: none !important;
}
.toolbar-top.no-shadow:before,
.ios .toolbar-top-ios.no-shadow:before,
.md .toolbar-top-md.no-shadow:before,
.aurora .toolbar-top-aurora.no-shadow:before,
.toolbar-top.toolbar-hidden:before,
.ios .toolbar-top-ios.toolbar-hidden:before,
.md .toolbar-top-md.toolbar-hidden:before,
.aurora .toolbar-top-aurora.toolbar-hidden:before {
  display: none !important;
}
.toolbar-top:after,
.ios .toolbar-top-ios:after,
.md .toolbar-top-md:after,
.aurora .toolbar-top-aurora:after,
.toolbar-top:before,
.ios .toolbar-top-ios:before,
.md .toolbar-top-md:before,
.aurora .toolbar-top-aurora:before {
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.toolbar-top:after,
.ios .toolbar-top-ios:after,
.md .toolbar-top-md:after,
.aurora .toolbar-top-aurora:after {
  content: '';
  position: absolute;
  background-color: var(--f7-toolbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.toolbar-top:before,
.ios .toolbar-top-ios:before,
.md .toolbar-top-md:before,
.aurora .toolbar-top-aurora:before {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  top: 100%;
  bottom: auto;
  height: 8px;
  pointer-events: none;
  background: var(--f7-toolbar-top-shadow-image);
}
.toolbar-bottom,
.ios .toolbar-bottom-ios,
.md .toolbar-bottom-md,
.aurora .toolbar-bottom-aurora {
  bottom: 0;
  height: calc(var(--f7-toolbar-height) + var(--f7-safe-area-bottom));
}
.toolbar-bottom .tab-link-highlight,
.ios .toolbar-bottom-ios .tab-link-highlight,
.md .toolbar-bottom-md .tab-link-highlight,
.aurora .toolbar-bottom-aurora .tab-link-highlight {
  top: 0;
}
.toolbar-bottom .toolbar-inner,
.ios .toolbar-bottom-ios .toolbar-inner,
.md .toolbar-bottom-md .toolbar-inner,
.aurora .toolbar-bottom-aurora .toolbar-inner {
  height: auto;
  top: 0;
  bottom: var(--f7-safe-area-bottom);
}
.toolbar-bottom.no-hairline:before,
.ios .toolbar-bottom-ios.no-hairline:before,
.md .toolbar-bottom-md.no-hairline:before,
.aurora .toolbar-bottom-aurora.no-hairline:before,
.toolbar-bottom.no-border:before,
.ios .toolbar-bottom-ios.no-border:before,
.md .toolbar-bottom-md.no-border:before,
.aurora .toolbar-bottom-aurora.no-border:before {
  display: none !important;
}
.toolbar-bottom.no-shadow:after,
.ios .toolbar-bottom-ios.no-shadow:after,
.md .toolbar-bottom-md.no-shadow:after,
.aurora .toolbar-bottom-aurora.no-shadow:after,
.toolbar-bottom.toolbar-hidden:after,
.ios .toolbar-bottom-ios.toolbar-hidden:after,
.md .toolbar-bottom-md.toolbar-hidden:after,
.aurora .toolbar-bottom-aurora.toolbar-hidden:after {
  display: none !important;
}
.toolbar-bottom:before,
.ios .toolbar-bottom-ios:before,
.md .toolbar-bottom-md:before,
.aurora .toolbar-bottom-aurora:before {
  content: '';
  position: absolute;
  background-color: var(--f7-toolbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.toolbar-bottom:after,
.ios .toolbar-bottom-ios:after,
.md .toolbar-bottom-md:after,
.aurora .toolbar-bottom-aurora:after {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  bottom: 100%;
  height: 8px;
  top: auto;
  pointer-events: none;
  background: var(--f7-toolbar-bottom-shadow-image);
}
.toolbar-inner {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
  align-items: center;
  align-content: center;
  overflow: hidden;
  padding: 0 calc(var(--f7-toolbar-inner-padding-right) + var(--f7-safe-area-right)) 0 calc(var(--f7-toolbar-inner-padding-left) + var(--f7-safe-area-left));
}
.views > .tabbar,
.views > .tabbar-labels {
  z-index: 5001;
}
.tabbar a,
.tabbar-labels a {
  color: var(--f7-tabbar-link-inactive-color);
}
.tabbar .tab-link:not(.tab-link-active),
.tabbar-labels .tab-link:not(.tab-link-active) {
  background-color: var(--f7-tabbar-link-inactive-bg-color, transparent);
}
.tabbar .link,
.tabbar-labels .link {
  line-height: 1.4;
}
.tabbar .tab-link,
.tabbar-labels .tab-link,
.tabbar .link,
.tabbar-labels .link {
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-transform: var(--f7-tabbar-link-text-transform);
  font-weight: var(--f7-tabbar-link-font-weight);
  letter-spacing: var(--f7-tabbar-link-letter-spacing);
  overflow: hidden;
}
.tabbar .tab-link-active,
.tabbar-labels .tab-link-active {
  color: var(--f7-tabbar-link-active-color, var(--f7-theme-color));
  background-color: var(--f7-tabbar-link-active-bg-color, transparent);
}
.tabbar i.icon,
.tabbar-labels i.icon {
  font-size: var(--f7-tabbar-icon-size);
  height: var(--f7-tabbar-icon-size);
  line-height: var(--f7-tabbar-icon-size);
}
.tabbar-labels {
  --f7-toolbar-height: var(--f7-tabbar-labels-height);
}
.tabbar-labels .tab-link,
.tabbar-labels .link {
  height: 100%;
  justify-content: space-between;
  align-items: center;
}
.tabbar-labels .tabbar-label {
  display: block;
  line-height: 1;
  margin: 0;
  position: relative;
  text-overflow: ellipsis;
  white-space: nowrap;
  font-size: var(--f7-tabbar-label-font-size);
  text-transform: var(--f7-tabbar-label-text-transform);
  font-weight: var(--f7-tabbar-label-font-weight);
  letter-spacing: var(--f7-tabbar-label-letter-spacing);
}
@media (min-width: 768px) and (min-height: 600px) {
  :root {
    --f7-tabbar-labels-height: var(--f7-tabbar-labels-tablet-height);
    --f7-tabbar-label-font-size: var(--f7-tabbar-label-tablet-font-size);
  }
}
.tabbar-scrollable .toolbar-inner {
  justify-content: flex-start;
  overflow: auto;
  -webkit-overflow-scrolling: touch;
}
.tabbar-scrollable .toolbar-inner::-webkit-scrollbar {
  display: none !important;
  width: 0 !important;
  height: 0 !important;
  -webkit-appearance: none;
  opacity: 0 !important;
}
.tabbar-scrollable .tab-link,
.tabbar-scrollable .link {
  width: auto;
  flex-shrink: 0;
}
.toolbar-transitioning,
.navbar-transitioning + .toolbar,
.navbar-transitioning ~ * .toolbar {
  transition-duration: var(--f7-toolbar-hide-show-transition-duration);
}
.toolbar-bottom ~ *,
.ios .toolbar-bottom-ios ~ *,
.md .toolbar-bottom-md ~ *,
.aurora .toolbar-bottom-aurora ~ * {
  --f7-page-toolbar-bottom-offset: var(--f7-toolbar-height);
}
.toolbar-bottom.tabbar-labels ~ *,
.ios .toolbar-bottom-ios.tabbar-labels ~ *,
.md .toolbar-bottom-md.tabbar-labels ~ *,
.aurora .toolbar-bottom-aurora.tabbar-labels ~ * {
  --f7-page-toolbar-bottom-offset: var(--f7-tabbar-labels-height);
}
.toolbar-bottom.toolbar-hidden,
.ios .toolbar-bottom-ios.toolbar-hidden,
.md .toolbar-bottom-md.toolbar-hidden,
.aurora .toolbar-bottom-aurora.toolbar-hidden {
  transform: translate3d(0, 100%, 0);
}
.toolbar-top ~ *,
.ios .toolbar-top-ios ~ *,
.md .toolbar-top-md ~ *,
.aurora .toolbar-top-aurora ~ * {
  --f7-page-toolbar-top-offset: var(--f7-toolbar-height);
}
.toolbar-top.tabbar-labels ~ *,
.ios .toolbar-top-ios.tabbar-labels ~ *,
.md .toolbar-top-md.tabbar-labels ~ *,
.aurora .toolbar-top-aurora.tabbar-labels ~ * {
  --f7-page-toolbar-top-offset: var(--f7-tabbar-labels-height);
}
.toolbar-top.toolbar-hidden,
.ios .toolbar-top-ios.toolbar-hidden,
.md .toolbar-top-md.toolbar-hidden,
.aurora .toolbar-top-aurora.toolbar-hidden {
  transform: translate3d(0, -100%, 0);
}
.navbar ~ .toolbar-top,
.navbars ~ .toolbar-top,
.ios .navbar ~ .toolbar-top-ios,
.ios .navbars ~ .toolbar-top-ios,
.md .navbar ~ .toolbar-top-md,
.aurora .navbar ~ .toolbar-top-aurora,
.navbar ~ * .toolbar-top,
.navbars ~ * .toolbar-top,
.ios .navbar ~ * .toolbar-top-ios,
.ios .navbars ~ * .toolbar-top-ios,
.md .navbar ~ * .toolbar-top-md,
.aurora .navbar ~ * .toolbar-top-aurora,
.navbar ~ .page:not(.no-navbar) .toolbar-top,
.navbars ~ .page:not(.no-navbar) .toolbar-top,
.ios .navbar ~ .page:not(.no-navbar) .toolbar-top-ios,
.ios .navbars ~ .page:not(.no-navbar) .toolbar-top-ios,
.md .navbar ~ .page:not(.no-navbar) .toolbar-top-md,
.aurora .navbar ~ .page:not(.no-navbar) .toolbar-top-aurora {
  top: calc(var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbar ~ .toolbar-top.toolbar-hidden,
.navbars ~ .toolbar-top.toolbar-hidden,
.ios .navbar ~ .toolbar-top-ios.toolbar-hidden,
.ios .navbars ~ .toolbar-top-ios.toolbar-hidden,
.md .navbar ~ .toolbar-top-md.toolbar-hidden,
.aurora .navbar ~ .toolbar-top-aurora.toolbar-hidden,
.navbar ~ * .toolbar-top.toolbar-hidden,
.navbars ~ * .toolbar-top.toolbar-hidden,
.ios .navbar ~ * .toolbar-top-ios.toolbar-hidden,
.ios .navbars ~ * .toolbar-top-ios.toolbar-hidden,
.md .navbar ~ * .toolbar-top-md.toolbar-hidden,
.aurora .navbar ~ * .toolbar-top-aurora.toolbar-hidden,
.navbar ~ .page:not(.no-navbar) .toolbar-top.toolbar-hidden,
.navbars ~ .page:not(.no-navbar) .toolbar-top.toolbar-hidden,
.ios .navbar ~ .page:not(.no-navbar) .toolbar-top-ios.toolbar-hidden,
.ios .navbars ~ .page:not(.no-navbar) .toolbar-top-ios.toolbar-hidden,
.md .navbar ~ .page:not(.no-navbar) .toolbar-top-md.toolbar-hidden,
.aurora .navbar ~ .page:not(.no-navbar) .toolbar-top-aurora.toolbar-hidden {
  transform: translate3d(0, calc(-1 * (var(--f7-navbar-height) + var(--f7-toolbar-height) + var(--f7-safe-area-top))), 0);
}
.navbar ~ .toolbar-top.toolbar-hidden.tabbar-labels,
.navbars ~ .toolbar-top.toolbar-hidden.tabbar-labels,
.ios .navbar ~ .toolbar-top-ios.toolbar-hidden.tabbar-labels,
.ios .navbars ~ .toolbar-top-ios.toolbar-hidden.tabbar-labels,
.md .navbar ~ .toolbar-top-md.toolbar-hidden.tabbar-labels,
.aurora .navbar ~ .toolbar-top-aurora.toolbar-hidden.tabbar-labels,
.navbar ~ * .toolbar-top.toolbar-hidden.tabbar-labels,
.navbars ~ * .toolbar-top.toolbar-hidden.tabbar-labels,
.ios .navbar ~ * .toolbar-top-ios.toolbar-hidden.tabbar-labels,
.ios .navbars ~ * .toolbar-top-ios.toolbar-hidden.tabbar-labels,
.md .navbar ~ * .toolbar-top-md.toolbar-hidden.tabbar-labels,
.aurora .navbar ~ * .toolbar-top-aurora.toolbar-hidden.tabbar-labels,
.navbar ~ .page:not(.no-navbar) .toolbar-top.toolbar-hidden.tabbar-labels,
.navbars ~ .page:not(.no-navbar) .toolbar-top.toolbar-hidden.tabbar-labels,
.ios .navbar ~ .page:not(.no-navbar) .toolbar-top-ios.toolbar-hidden.tabbar-labels,
.ios .navbars ~ .page:not(.no-navbar) .toolbar-top-ios.toolbar-hidden.tabbar-labels,
.md .navbar ~ .page:not(.no-navbar) .toolbar-top-md.toolbar-hidden.tabbar-labels,
.aurora .navbar ~ .page:not(.no-navbar) .toolbar-top-aurora.toolbar-hidden.tabbar-labels {
  transform: translate3d(0, calc(-1 * (var(--f7-navbar-height) + var(--f7-tabbar-labels-height) + var(--f7-safe-area-top))), 0);
}
.navbar-hidden + .toolbar-top:not(.toolbar-hidden),
.ios .navbar-hidden + .toolbar-top-ios:not(.toolbar-hidden),
.md .navbar-hidden + .toolbar-top-md:not(.toolbar-hidden),
.aurora .navbar-hidden + .toolbar-top-aurora:not(.toolbar-hidden),
.navbar-hidden ~ * .toolbar-top:not(.toolbar-hidden),
.ios .navbar-hidden ~ * .toolbar-top-ios:not(.toolbar-hidden),
.md .navbar-hidden ~ * .toolbar-top-md:not(.toolbar-hidden),
.aurora .navbar-hidden ~ * .toolbar-top-aurora:not(.toolbar-hidden) {
  transform: translate3d(0, calc(0px - var(--f7-navbar-height)), 0);
}
.navbar-large-hidden + .toolbar-top:not(.toolbar-hidden),
.ios .navbar-large-hidden + .toolbar-top-ios:not(.toolbar-hidden),
.md .navbar-large-hidden + .toolbar-top-md:not(.toolbar-hidden),
.navbar-large-hidden ~ * .toolbar-top:not(.toolbar-hidden),
.ios .navbar-large-hidden ~ * .toolbar-top-ios:not(.toolbar-hidden),
.md .navbar-large-hidden ~ * .toolbar-top-md:not(.toolbar-hidden),
.aurora .navbar-large-hidden ~ * .toolbar-top-aurora:not(.toolbar-hidden) {
  transform: translate3d(0, calc(0px - var(--f7-navbar-height) - var(--f7-navbar-large-title-height)), 0);
}
.ios .toolbar a.icon-only {
  min-height: var(--f7-toolbar-height);
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
  min-width: 44px;
}
.ios .tabbar-labels .tab-link,
.ios .tabbar-labels .link {
  padding-top: 4px;
  padding-bottom: 4px;
}
.ios .tabbar-labels .tab-link i + span,
.ios .tabbar-labels .link i + span {
  margin: 0;
}
@media (min-width: 768px) and (min-height: 600px) {
  .ios .tabbar .tab-link,
  .ios .tabbar-labels .tab-link,
  .ios .tabbar .link,
  .ios .tabbar-labels .link {
    justify-content: center;
    flex-direction: row;
  }
  .ios .tabbar .tab-link i + span,
  .ios .tabbar-labels .tab-link i + span,
  .ios .tabbar .link i + span,
  .ios .tabbar-labels .link i + span {
    margin-left: 5px;
  }
}
.ios .tabbar-scrollable .toolbar-inner {
  justify-content: flex-start;
}
.ios .tabbar-scrollable .tab-link,
.ios .tabbar-scrollable .link {
  padding: 0 8px;
}
.md .toolbar .link {
  justify-content: center;
  padding: 0 16px;
  min-width: 48px;
}
.md .toolbar .link:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .toolbar .link.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .toolbar a.icon-only {
  min-width: 0;
  flex-shrink: 0;
}
.md .tabbar .tab-link,
.md .tabbar-labels .tab-link,
.md .tabbar .link,
.md .tabbar-labels .link {
  padding-left: 0;
  padding-right: 0;
}
.md .tabbar a.icon-only,
.md .tabbar-labels a.icon-only {
  flex-shrink: initial;
}
.md .tabbar .tab-link,
.md .tabbar-labels .tab-link {
  transition-duration: 300ms;
  overflow: hidden;
  position: relative;
}
.md .tabbar .tab-link-highlight,
.md .tabbar-labels .tab-link-highlight {
  position: absolute;
  height: 2px;
  background: var(--f7-tabbar-link-active-border-color, var(--f7-theme-color));
  transition-duration: 300ms;
  left: 0;
}
.md .tabbar-labels .tab-link,
.md .tabbar-labels .link {
  padding-top: 7px;
  padding-bottom: 7px;
}
.md .tabbar-label {
  max-width: 100%;
  overflow: hidden;
  line-height: 1.2;
}
.md .tabbar-scrollable .toolbar-inner {
  overflow: auto;
}
.md .tabbar-scrollable .tab-link,
.md .tabbar-scrollable .link {
  padding: 0 16px;
}
.aurora .toolbar a.icon-only {
  min-height: var(--f7-toolbar-height);
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
}
.aurora .tabbar .toolbar-inner,
.aurora .tabbar-labels .toolbar-inner {
  padding-left: 0;
  padding-right: 0;
}
.aurora .tabbar .tab-link,
.aurora .tabbar-labels .tab-link,
.aurora .tabbar .link,
.aurora .tabbar-labels .link {
  transition-duration: 200ms;
}
.aurora .tabbar-labels .tab-link,
.aurora .tabbar-labels .link {
  padding-top: 5px;
  padding-bottom: 5px;
}
.aurora .tabbar-labels .tab-link i + span,
.aurora .tabbar-labels .link i + span {
  margin: 0;
}
.aurora .tabbar-scrollable .toolbar-inner {
  justify-content: flex-start;
}
.aurora .tabbar-scrollable .tab-link,
.aurora .tabbar-scrollable .link {
  padding: 0 16px;
}
/* === Subnavbar === */
:root {
  /*
  --f7-subnavbar-bg-image: var(--f7-bars-bg-image);
  --f7-subnavbar-bg-color: var(--f7-bars-bg-color);
  --f7-subnavbar-bg-color-rgb: var(--f7-bars-bg-color-rgb);
  --f7-subnavbar-border-color: var(--f7-bars-border-color);
  --f7-subnavbar-link-color: var(--f7-bars-link-color);
  --f7-subnavbar-text-color: var(--f7-bars-text-color);
  */
  --f7-subnavbar-title-line-height: 1.2;
}
.ios {
  --f7-subnavbar-height: 44px;
  --f7-subnavbar-inner-padding-left: 8px;
  --f7-subnavbar-inner-padding-right: 8px;
  --f7-subnavbar-title-font-size: 34px;
  --f7-subnavbar-title-font-weight: 700;
  --f7-subnavbar-title-letter-spacing: -0.03em;
  --f7-subnavbar-title-margin-left: 8px;
  --f7-subnavbar-shadow-image: none;
  /*
  --f7-subnavbar-link-height: var(--f7-subnavbar-height);
  --f7-subnavbar-link-line-height: var(--f7-subnavbar-height);
  */
}
.md {
  --f7-subnavbar-height: 48px;
  --f7-subnavbar-inner-padding-left: 16px;
  --f7-subnavbar-inner-padding-right: 16px;
  --f7-subnavbar-title-font-size: 20px;
  --f7-subnavbar-title-font-weight: 500;
  --f7-subnavbar-title-letter-spacing: 0;
  --f7-subnavbar-title-margin-left: 0px;
  --f7-subnavbar-shadow-image: var(--f7-bars-shadow-bottom-image);
  /*
  --f7-subnavbar-link-height: var(--f7-subnavbar-height);
  --f7-subnavbar-link-line-height: var(--f7-subnavbar-height);
  */
}
.aurora {
  --f7-subnavbar-height: 38px;
  --f7-subnavbar-inner-padding-left: 16px;
  --f7-subnavbar-inner-padding-right: 16px;
  --f7-subnavbar-title-font-size: 26px;
  --f7-subnavbar-title-font-weight: bold;
  --f7-subnavbar-title-letter-spacing: -0.03em;
  --f7-subnavbar-title-margin-left: 0px;
  --f7-subnavbar-shadow-image: none;
  --f7-subnavbar-link-height: auto;
  --f7-subnavbar-link-line-height: inherit;
}
.subnavbar {
  width: 100%;
  position: absolute;
  left: 0;
  top: 0;
  z-index: 600;
  box-sizing: border-box;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-image: var(--f7-subnavbar-bg-image, var(--f7-bars-bg-image));
  background-color: var(--f7-subnavbar-bg-color, var(--f7-bars-bg-color));
  color: var(--f7-subnavbar-text-color, var(--f7-bars-text-color));
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .subnavbar {
    background-color: rgba(var(--f7-subnavbar-bg-color-rgb, var(--f7-bars-bg-color-rgb)), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.subnavbar .subnavbar-title {
  position: relative;
  overflow: hidden;
  text-overflow: ellpsis;
  white-space: nowrap;
  font-size: var(--f7-subnavbar-title-font-size);
  font-weight: var(--f7-subnavbar-title-font-weight);
  text-align: left;
  display: inline-block;
  line-height: var(--f7-subnavbar-title-line-height);
  letter-spacing: var(--f7-subnavbar-title-letter-spacing);
  margin-left: var(--f7-subnavbar-title-margin-left);
}
.subnavbar .left,
.subnavbar .right {
  flex-shrink: 0;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
.subnavbar .right:first-child {
  position: absolute;
  height: 100%;
}
.subnavbar a {
  color: var(--f7-subnavbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.subnavbar a.link {
  line-height: var(--f7-subnavbar-link-line-height, var(--f7-subnavbar-height));
  height: var(--f7-subnavbar-link-height, var(--f7-subnavbar-height));
}
.subnavbar a.icon-only {
  min-width: var(--f7-subnavbar-height);
}
.subnavbar.no-hairline:after,
.subnavbar.no-border:after {
  display: none !important;
}
.subnavbar.no-shadow:before,
.subnavbar.navbar-hidden:before {
  display: none !important;
}
.subnavbar:after,
.subnavbar:before {
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.subnavbar:after {
  content: '';
  position: absolute;
  background-color: var(--f7-subnavbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.subnavbar:before {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  top: 100%;
  bottom: auto;
  height: 8px;
  pointer-events: none;
  background: var(--f7-subnavbar-shadow-image);
}
.subnavbar-inner {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  box-sizing: border-box;
  justify-content: space-between;
  overflow: hidden;
  padding: 0 calc(var(--f7-subnavbar-inner-padding-left) + var(--f7-safe-area-right)) 0 calc(var(--f7-subnavbar-inner-padding-right) + var(--f7-safe-area-left));
}
.subnavbar-inner.stacked {
  display: none;
}
.navbar .subnavbar {
  top: 100%;
}
.views > .subnavbar,
.view > .subnavbar,
.page > .subnavbar {
  position: absolute;
}
.navbar ~ * .subnavbar,
.navbars ~ * .subnavbar,
.page-with-subnavbar .navbar ~ .subnavbar,
.page-with-subnavbar .navbar ~ * .subnavbar,
.navbar ~ .page-with-subnavbar:not(.no-navbar) .subnavbar,
.navbar ~ .subnavbar,
.navbars ~ .page-with-subnavbar:not(.no-navbar) .subnavbar,
.navbars ~ .subnavbar {
  top: calc(var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbar ~ .page-with-navbar-large:not(.no-navbar) .subnavbar,
.navbars ~ .page-with-navbar-large:not(.no-navbar) .subnavbar,
.page-with-subnavbar.page-with-navbar-large .navbar ~ .subnavbar,
.page-with-subnavbar.page-with-navbar-large .navbar ~ * .subnavbar,
.navbar .title-large ~ .subnavbar {
  top: calc(var(--f7-navbar-height) + var(--f7-navbar-large-title-height) + var(--f7-safe-area-top));
  transform: translate3d(0, calc(-1 * var(--f7-navbar-large-collapse-progress) * var(--f7-navbar-large-title-height)), 0);
}
.page-with-subnavbar,
.subnavbar ~ * {
  --f7-page-subnavbar-offset: var(--f7-subnavbar-height);
}
.ios .subnavbar {
  height: calc(var(--f7-subnavbar-height) + 1px);
  margin-top: -1px;
  padding-top: 1px;
}
.ios .subnavbar .title {
  align-self: flex-start;
  flex-shrink: 10;
}
.ios .subnavbar .left a + a,
.ios .subnavbar .right a + a {
  margin-left: 16px;
}
.ios .subnavbar .left {
  margin-right: 10px;
}
.ios .subnavbar .right {
  margin-left: 10px;
}
.ios .subnavbar .right:first-child {
  right: 8px;
}
.ios .subnavbar a.link {
  justify-content: flex-start;
}
.ios .subnavbar a.icon-only {
  justify-content: center;
  margin: 0;
}
.md .subnavbar {
  height: var(--f7-subnavbar-height);
}
.md .subnavbar .right {
  margin-left: auto;
}
.md .subnavbar .right:first-child {
  right: 16px;
}
.md .subnavbar a.link {
  justify-content: center;
  padding: 0 16px;
}
.md .subnavbar a.link:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .subnavbar a.link.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .subnavbar a.icon-only {
  flex-shrink: 0;
}
.md .subnavbar-inner > a.link:first-child {
  margin-left: calc(-1 * var(--f7-subnavbar-inner-padding-left));
}
.md .subnavbar-inner > a.link:last-child {
  margin-right: calc(-1 * var(--f7-subnavbar-inner-padding-right));
}
.aurora .subnavbar {
  height: calc(var(--f7-subnavbar-height) + 1px);
  margin-top: -1px;
  padding-top: 1px;
}
.aurora .subnavbar .title {
  align-self: flex-start;
  flex-shrink: 10;
}
.aurora .subnavbar .left a + a,
.aurora .subnavbar .right a + a {
  margin-left: 10px;
}
.aurora .subnavbar .left {
  margin-right: 10px;
}
.aurora .subnavbar .right {
  margin-left: 10px;
}
.aurora .subnavbar .right:first-child {
  right: 16px;
}
.aurora .subnavbar a.link {
  justify-content: flex-start;
}
.aurora .subnavbar a.icon-only {
  justify-content: center;
  margin: 0;
}
/* === Content Block === */
:root {
  --f7-block-padding-horizontal: 16px;
  --f7-block-padding-vertical: 16px;
  --f7-block-font-size: inherit;
  --f7-block-text-color: inherit;
  --f7-block-header-margin: 10px;
  --f7-block-footer-margin: 10px;
  --f7-block-header-font-size: 14px;
  --f7-block-footer-font-size: 14px;
  --f7-block-title-text-transform: none;
  --f7-block-title-white-space: nowrap;
  --f7-block-title-medium-text-transform: none;
  --f7-block-title-large-text-transform: none;
  --f7-block-inset-side-margin: 16px;
  --f7-block-title-medium-text-color: #000;
  --f7-block-title-large-text-color: #000;
  --f7-block-strong-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-block-title-text-color: #fff;
  --f7-block-strong-border-color: rgba(255, 255, 255, 0.15);
  --f7-block-title-medium-text-color: #fff;
  --f7-block-title-large-text-color: #fff;
  --f7-block-strong-bg-color: #1c1c1d;
}
.ios {
  --f7-block-margin-vertical: 35px;
  --f7-block-strong-border-color: rgba(0, 0, 0, 0.22);
  --f7-block-title-text-color: #000;
  --f7-block-title-font-size: 16px;
  --f7-block-title-font-weight: 600;
  --f7-block-title-line-height: 20px;
  --f7-block-title-margin-bottom: 10px;
  --f7-block-title-medium-font-size: 22px;
  --f7-block-title-medium-font-weight: bold;
  --f7-block-title-medium-line-height: 1.4;
  --f7-block-title-large-font-size: 30px;
  --f7-block-title-large-font-weight: bold;
  --f7-block-title-large-line-height: 1.3;
  --f7-block-inset-border-radius: 8px;
  --f7-block-strong-text-color: #000;
  --f7-block-header-text-color: rgba(0, 0, 0, 0.45);
  --f7-block-footer-text-color: rgba(0, 0, 0, 0.45);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-block-header-text-color: rgba(255, 255, 255, 0.55);
  --f7-block-footer-text-color: rgba(255, 255, 255, 0.55);
  --f7-block-strong-text-color: #fff;
}
.md {
  --f7-block-margin-vertical: 32px;
  --f7-block-strong-text-color: inherit;
  --f7-block-strong-border-color: rgba(0, 0, 0, 0.12);
  --f7-block-title-font-size: inherit;
  --f7-block-title-text-color: rgba(0, 0, 0, 0.54);
  --f7-block-title-font-weight: 500;
  --f7-block-title-line-height: 16px;
  --f7-block-title-margin-bottom: 16px;
  --f7-block-title-medium-font-size: 24px;
  --f7-block-title-medium-font-weight: 500;
  --f7-block-title-medium-line-height: 1.3;
  --f7-block-title-large-font-size: 34px;
  --f7-block-title-large-font-weight: 500;
  --f7-block-title-large-line-height: 1.2;
  --f7-block-inset-border-radius: 4px;
  --f7-block-header-text-color: rgba(0, 0, 0, 0.54);
  --f7-block-footer-text-color: rgba(0, 0, 0, 0.54);
}
.md .theme-dark,
.md.theme-dark {
  --f7-block-header-text-color: rgba(255, 255, 255, 0.54);
  --f7-block-footer-text-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-block-margin-vertical: 15px;
  --f7-block-strong-border-color: rgba(0, 0, 0, 0.12);
  --f7-block-title-font-size: inherit;
  --f7-block-title-text-color: rgba(0, 0, 0, 0.7);
  --f7-block-title-font-weight: 600;
  --f7-block-title-line-height: 1.5;
  --f7-block-title-margin-bottom: 5px;
  --f7-block-title-medium-font-size: 20px;
  --f7-block-title-medium-font-weight: 600;
  --f7-block-title-medium-line-height: 1.4;
  --f7-block-title-large-font-size: 28px;
  --f7-block-title-large-font-weight: bold;
  --f7-block-title-large-line-height: 1.3;
  --f7-block-inset-border-radius: 4px;
  --f7-block-strong-text-color: inherit;
  --f7-block-header-text-color: rgba(0, 0, 0, 0.6);
  --f7-block-footer-text-color: rgba(0, 0, 0, 0.6);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-block-header-text-color: rgba(255, 255, 255, 0.54);
  --f7-block-footer-text-color: rgba(255, 255, 255, 0.54);
  --f7-block-strong-text-color: #fff;
}
.block {
  box-sizing: border-box;
  position: relative;
  z-index: 1;
  color: var(--f7-block-text-color);
  margin: var(--f7-block-margin-vertical) 0;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: calc(var(--f7-block-padding-horizontal) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-block-padding-horizontal) + var(--f7-safe-area-right));
  font-size: var(--f7-block-font-size);
}
.block.no-hairlines:before,
.block.no-hairlines ul:before,
.md .block.no-hairlines-md:before,
.md .block.no-hairlines-md ul:before,
.ios .block.no-hairlines-ios:before,
.ios .block.no-hairlines-ios ul:before,
.aurora .block.no-hairlines-aurora:before,
.aurora .block.no-hairlines-aurora ul:before,
.block.no-hairlines:after,
.block.no-hairlines ul:after,
.md .block.no-hairlines-md:after,
.md .block.no-hairlines-md ul:after,
.ios .block.no-hairlines-ios:after,
.ios .block.no-hairlines-ios ul:after,
.aurora .block.no-hairlines-aurora:after,
.aurora .block.no-hairlines-aurora ul:after {
  display: none !important;
}
.block.no-hairline-top:before,
.block.no-hairline-top ul:before,
.md .block.no-hairline-top-md:before,
.md .block.no-hairline-top-md ul:before,
.ios .block.no-hairline-top-ios:before,
.ios .block.no-hairline-top-ios ul:before,
.aurora .block.no-hairline-top-aurora:before,
.aurora .block.no-hairline-top-aurora ul:before {
  display: none !important;
}
.block.no-hairline-bottom:after,
.block.no-hairline-bottom ul:after,
.md .block.no-hairline-bottom-md:after,
.md .block.no-hairline-bottom-md ul:after,
.ios .block.no-hairline-bottom-ios:after,
.ios .block.no-hairline-bottom-ios ul:after,
.aurora .block.no-hairline-bottom-aurora:after,
.aurora .block.no-hairline-bottom-aurora ul:after {
  display: none !important;
}
.block > h1:first-child,
.block > h2:first-child,
.block > h3:first-child,
.block > h4:first-child,
.block > p:first-child {
  margin-top: 0;
}
.block > h1:last-child,
.block > h2:last-child,
.block > h3:last-child,
.block > h4:last-child,
.block > p:last-child {
  margin-bottom: 0;
}
.block-strong {
  color: var(--f7-block-strong-text-color);
  padding-top: var(--f7-block-padding-vertical);
  padding-bottom: var(--f7-block-padding-vertical);
  background-color: var(--f7-block-strong-bg-color);
}
.block-strong:before {
  content: '';
  position: absolute;
  background-color: var(--f7-block-strong-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.block-strong:after {
  content: '';
  position: absolute;
  background-color: var(--f7-block-strong-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.block-title {
  position: relative;
  overflow: hidden;
  margin: 0;
  white-space: var(--f7-block-title-white-space);
  text-overflow: ellipsis;
  text-transform: var(--f7-block-title-text-transform);
  color: var(--f7-block-title-text-color);
  font-size: var(--f7-block-title-font-size, inherit);
  font-weight: var(--f7-block-title-font-weight);
  line-height: var(--f7-block-title-line-height);
  margin-top: var(--f7-block-margin-vertical);
  margin-bottom: var(--f7-block-title-margin-bottom);
  margin-left: calc(var(--f7-block-padding-horizontal) + var(--f7-safe-area-left));
  margin-right: calc(var(--f7-block-padding-horizontal) + var(--f7-safe-area-right));
}
.block-title + .list,
.block-title + .block,
.block-title + .card,
.block-title + .timeline,
.block-title + .block-header {
  margin-top: 0px;
}
.block-title-medium {
  font-size: var(--f7-block-title-medium-font-size);
  text-transform: var(--f7-block-title-medium-text-transform);
  color: var(--f7-block-title-medium-text-color);
  font-weight: var(--f7-block-title-medium-font-weight);
  line-height: var(--f7-block-title-medium-line-height);
}
.block-title-large {
  font-size: var(--f7-block-title-large-font-size);
  text-transform: var(--f7-block-title-large-text-transform);
  color: var(--f7-block-title-large-text-color);
  font-weight: var(--f7-block-title-large-font-weight);
  line-height: var(--f7-block-title-large-line-height);
}
.block > .block-title:first-child,
.list > .block-title:first-child {
  margin-top: 0;
  margin-left: 0;
  margin-right: 0;
}
.block-header {
  color: var(--f7-block-header-text-color);
  font-size: var(--f7-block-header-font-size);
  margin-bottom: var(--f7-block-header-margin);
  margin-top: var(--f7-block-margin-vertical);
}
.block-header + .list,
.block-header + .block,
.block-header + .card,
.block-header + .timeline {
  margin-top: var(--f7-block-header-margin);
}
.block-footer {
  color: var(--f7-block-footer-text-color);
  font-size: var(--f7-block-footer-font-size);
  margin-top: var(--f7-block-footer-margin);
  margin-bottom: var(--f7-block-margin-vertical);
}
.block-footer,
.block-header {
  padding-top: 0;
  padding-bottom: 0;
  padding-left: calc(var(--f7-block-padding-horizontal) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-block-padding-horizontal) + var(--f7-safe-area-right));
}
.block-footer ul:first-child,
.block-header ul:first-child,
.block-footer p:first-child,
.block-header p:first-child,
.block-footer h1:first-child,
.block-header h1:first-child,
.block-footer h2:first-child,
.block-header h2:first-child,
.block-footer h3:first-child,
.block-header h3:first-child,
.block-footer h4:first-child,
.block-header h4:first-child {
  margin-top: 0;
}
.block-footer ul:last-child,
.block-header ul:last-child,
.block-footer p:last-child,
.block-header p:last-child,
.block-footer h1:last-child,
.block-header h1:last-child,
.block-footer h2:last-child,
.block-header h2:last-child,
.block-footer h3:last-child,
.block-header h3:last-child,
.block-footer h4:last-child,
.block-header h4:last-child {
  margin-bottom: 0;
}
.block-footer ul:first-child:last-child,
.block-header ul:first-child:last-child,
.block-footer p:first-child:last-child,
.block-header p:first-child:last-child,
.block-footer h1:first-child:last-child,
.block-header h1:first-child:last-child,
.block-footer h2:first-child:last-child,
.block-header h2:first-child:last-child,
.block-footer h3:first-child:last-child,
.block-header h3:first-child:last-child,
.block-footer h4:first-child:last-child,
.block-header h4:first-child:last-child {
  margin-top: 0;
  margin-bottom: 0;
}
.list .block-header,
.block .block-header,
.card .block-header,
.timeline .block-header {
  margin-top: 0;
}
.list .block-footer,
.block .block-footer,
.card .block-footer,
.timeline .block-footer {
  margin-bottom: 0;
}
.list + .block-footer,
.block + .block-footer,
.card + .block-footer,
.timeline + .block-footer {
  margin-top: calc(-1 * (var(--f7-block-margin-vertical) - var(--f7-block-footer-margin)));
}
.block + .block-footer {
  margin-top: calc(-1 * (var(--f7-block-margin-vertical) - var(--f7-block-footer-margin)));
  margin-bottom: var(--f7-block-margin-vertical);
}
.block .block-header,
.block .block-footer {
  padding: 0;
}
.block.inset {
  border-radius: var(--f7-block-inset-border-radius);
  margin-left: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-left));
  margin-right: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-right));
  --f7-safe-area-left: 0px;
  --f7-safe-area-right: 0px;
}
.block-strong.inset:before,
.block-strong.inset:after {
  display: none !important;
}
@media (min-width: 480px) {
  .block.xsmall-inset {
    border-radius: var(--f7-block-inset-border-radius);
    margin-left: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-right));
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .block-strong.xsmall-inset:before,
  .block-strong.xsmall-inset:after {
    display: none !important;
  }
}
@media (min-width: 568px) {
  .block.small-inset {
    border-radius: var(--f7-block-inset-border-radius);
    margin-left: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-right));
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .block-strong.small-inset:before,
  .block-strong.small-inset:after {
    display: none !important;
  }
}
@media (min-width: 768px) {
  .block.medium-inset {
    border-radius: var(--f7-block-inset-border-radius);
    margin-left: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-right));
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .block-strong.medium-inset:before,
  .block-strong.medium-inset:after {
    display: none !important;
  }
}
@media (min-width: 1024px) {
  .block.large-inset {
    border-radius: var(--f7-block-inset-border-radius);
    margin-left: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-right));
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .block-strong.large-inset:before,
  .block-strong.large-inset:after {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .block.xlarge-inset {
    border-radius: var(--f7-block-inset-border-radius);
    margin-left: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-block-inset-side-margin) + var(--f7-safe-area-outer-right));
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .block-strong.xlarge-inset:before,
  .block-strong.xlarge-inset:after {
    display: none !important;
  }
}
/* === List View === */
:root {
  --f7-list-inset-side-margin: 16px;
  --f7-list-item-cell-margin: 16px;
  --f7-list-item-padding-horizontal: 16px;
  --f7-list-media-item-padding-horizontal: 16px;
  --f7-list-item-text-max-lines: 2;
  --f7-list-chevron-icon-font-size: 20px;
  --f7-list-item-title-font-size: inherit;
  --f7-list-item-title-font-weight: 400;
  --f7-list-item-title-text-color: inherit;
  --f7-list-item-title-line-height: inherit;
  --f7-list-item-title-white-space: nowrap;
  --f7-list-item-subtitle-font-weight: 400;
  --f7-list-item-subtitle-text-color: inherit;
  --f7-list-item-subtitle-line-height: inherit;
  --f7-list-item-text-font-weight: 400;
  --f7-list-item-after-font-weight: 400;
  --f7-list-item-header-text-color: inherit;
  --f7-list-item-header-font-size: 12px;
  --f7-list-item-header-font-weight: 400;
  --f7-list-item-header-line-height: 1.2;
  --f7-list-item-footer-font-size: 12px;
  --f7-list-item-footer-font-weight: 400;
  --f7-list-item-footer-line-height: 1.2;
  --f7-list-button-font-size: inherit;
  --f7-list-button-font-weight: 400;
  --f7-list-item-divider-line-height: inherit;
  --f7-list-group-title-line-height: inherit;
  --f7-list-bg-color: #fff;
  --f7-list-chevron-icon-color: rgba(0, 0, 0, 0.2);
}
:root .theme-dark,
:root.theme-dark {
  --f7-list-button-border-color: rgba(255, 255, 255, 0.15);
  --f7-list-bg-color: #1c1c1d;
  --f7-list-border-color: rgba(255, 255, 255, 0.15);
  --f7-list-item-border-color: rgba(255, 255, 255, 0.15);
  --f7-list-item-divider-border-color: rgba(255, 255, 255, 0.15);
  --f7-list-item-divider-bg-color: #232323;
  --f7-list-group-title-bg-color: #232323;
  --f7-list-chevron-icon-color: rgba(255, 255, 255, 0.3);
}
.ios {
  --f7-list-in-list-padding-left: 30px;
  --f7-list-inset-border-radius: 8px;
  --f7-list-margin-vertical: 35px;
  --f7-list-font-size: 17px;
  --f7-list-chevron-icon-area: 20px;
  --f7-list-border-color: rgba(0, 0, 0, 0.22);
  --f7-list-item-border-color: rgba(0, 0, 0, 0.22);
  --f7-list-link-pressed-bg-color: rgba(0, 0, 0, 0.15);
  --f7-list-item-subtitle-font-size: 15px;
  --f7-list-item-text-font-size: 15px;
  --f7-list-item-text-line-height: 21px;
  --f7-list-item-after-font-size: inherit;
  --f7-list-item-after-line-height: inherit;
  --f7-list-item-after-padding: 5px;
  --f7-list-item-min-height: 44px;
  --f7-list-item-media-margin: 16px;
  --f7-list-item-media-icons-margin: 5px;
  --f7-list-item-padding-vertical: 8px;
  --f7-list-media-item-padding-vertical: 10px;
  --f7-list-media-item-title-font-weight: 600;
  /*
  --f7-list-button-text-color: var(--f7-theme-color);
  */
  --f7-list-button-text-align: center;
  --f7-list-button-border-color: rgba(0, 0, 0, 0.22);
  --f7-list-item-divider-height: 31px;
  --f7-list-item-divider-font-size: inherit;
  --f7-list-item-divider-font-weight: 400;
  --f7-list-item-divider-bg-color: rgba(0, 0, 0, 0.03);
  --f7-list-item-divider-border-color: rgba(0, 0, 0, 0.22);
  --f7-list-group-title-height: 31px;
  --f7-list-group-title-font-size: inherit;
  --f7-list-group-title-font-weight: 400;
  --f7-list-group-title-bg-color: #f7f7f7;
  --f7-list-item-after-text-color: rgba(0, 0, 0, 0.45);
  --f7-list-item-footer-text-color: rgba(0, 0, 0, 0.45);
  --f7-list-item-text-text-color: rgba(0, 0, 0, 0.45);
  --f7-list-item-divider-text-color: rgba(0, 0, 0, 0.45);
  --f7-list-group-title-text-color: rgba(0, 0, 0, 0.45);
  --f7-list-button-pressed-bg-color: rgba(0, 0, 0, 0.15);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-list-item-after-text-color: rgba(255, 255, 255, 0.55);
  --f7-list-item-header-text-color: rgba(255, 255, 255, 0.55);
  --f7-list-item-footer-text-color: rgba(255, 255, 255, 0.55);
  --f7-list-item-text-text-color: rgba(255, 255, 255, 0.55);
  --f7-list-item-divider-text-color: rgba(255, 255, 255, 0.55);
  --f7-list-group-title-text-color: rgba(255, 255, 255, 0.55);
  --f7-list-link-pressed-bg-color: rgba(255, 255, 255, 0.08);
  --f7-list-button-pressed-bg-color: rgba(255, 255, 255, 0.08);
}
.md {
  --f7-list-in-list-padding-left: 40px;
  --f7-list-inset-border-radius: 4px;
  --f7-list-margin-vertical: 32px;
  --f7-list-font-size: 16px;
  --f7-list-chevron-icon-area: 26px;
  --f7-list-border-color: rgba(0, 0, 0, 0.12);
  --f7-list-item-border-color: rgba(0, 0, 0, 0.12);
  --f7-list-item-subtitle-font-size: 14px;
  --f7-list-item-text-font-size: 14px;
  --f7-list-item-text-line-height: 20px;
  --f7-list-item-after-font-size: 14px;
  --f7-list-item-after-line-height: inherit;
  --f7-list-item-after-padding: 8px;
  --f7-list-item-min-height: 48px;
  --f7-list-item-media-margin: 16px;
  --f7-list-item-media-icons-margin: 8px;
  --f7-list-item-padding-vertical: 8px;
  --f7-list-media-item-padding-vertical: 14px;
  /*
  --f7-list-media-item-title-font-weight: var(--f7-list-item-title-font-weight);
  */
  --f7-list-button-text-align: left;
  --f7-list-button-border-color: transparent;
  --f7-list-item-divider-height: 48px;
  --f7-list-item-divider-font-size: 14px;
  --f7-list-item-divider-font-weight: 400;
  --f7-list-item-divider-bg-color: #f4f4f4;
  --f7-list-item-divider-border-color: transparent;
  --f7-list-group-title-height: 48px;
  --f7-list-group-title-font-size: 14px;
  --f7-list-group-title-font-weight: 400;
  --f7-list-group-title-bg-color: #f4f4f4;
  --f7-list-link-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-list-item-text-text-color: rgba(0, 0, 0, 0.54);
  --f7-list-item-after-text-color: rgba(0, 0, 0, 0.54);
  --f7-list-item-footer-text-color: rgba(0, 0, 0, 0.5);
  --f7-list-button-text-color: #212121;
  --f7-list-button-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-list-item-divider-text-color: rgba(0, 0, 0, 0.54);
  --f7-list-group-title-text-color: rgba(0, 0, 0, 0.54);
}
.md .theme-dark,
.md.theme-dark {
  --f7-list-button-text-color: #fff;
  --f7-list-item-divider-text-color: #fff;
  --f7-list-group-title-text-color: #fff;
  --f7-list-link-pressed-bg-color: rgba(255, 255, 255, 0.05);
  --f7-list-button-pressed-bg-color: rgba(255, 255, 255, 0.05);
  --f7-list-item-text-text-color: rgba(255, 255, 255, 0.54);
  --f7-list-item-after-text-color: rgba(255, 255, 255, 0.54);
  --f7-list-item-footer-text-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-list-in-list-padding-left: 16px;
  --f7-list-inset-border-radius: 4px;
  --f7-list-margin-vertical: 15px;
  --f7-list-font-size: 14px;
  --f7-list-chevron-icon-area: 15px;
  --f7-list-chevron-icon-font-size: 16px;
  --f7-list-border-color: rgba(0, 0, 0, 0.12);
  --f7-list-item-border-color: rgba(0, 0, 0, 0.12);
  --f7-list-item-title-line-height: 1.3;
  --f7-list-item-subtitle-font-size: 14px;
  --f7-list-item-subtitle-line-height: 1.3;
  --f7-list-item-text-font-size: 12px;
  --f7-list-item-text-line-height: 16px;
  --f7-list-item-after-font-size: 13px;
  --f7-list-item-after-line-height: 1.2;
  --f7-list-item-after-padding: 5px;
  --f7-list-item-min-height: 32px;
  --f7-list-item-media-margin: 10px;
  --f7-list-item-media-icons-margin: 5px;
  --f7-list-item-padding-vertical: 5px;
  --f7-list-media-item-padding-vertical: 5px;
  --f7-list-media-item-title-font-weight: 600;
  /*
  --f7-list-button-text-color: var(--f7-theme-color);
  */
  --f7-list-button-text-align: center;
  --f7-list-button-border-color: rgba(0, 0, 0, 0.12);
  --f7-list-item-divider-height: 19px;
  --f7-list-item-divider-font-size: inherit;
  --f7-list-item-divider-font-weight: 500;
  --f7-list-item-divider-bg-color: rgba(0, 0, 0, 0.03);
  --f7-list-item-divider-border-color: transparent;
  --f7-list-group-title-height: 19px;
  --f7-list-group-title-font-size: inherit;
  --f7-list-group-title-font-weight: 500;
  --f7-list-group-title-bg-color: #f7f7f7;
  --f7-list-link-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-list-link-hover-bg-color: rgba(0, 0, 0, 0.03);
  --f7-list-item-text-text-color: rgba(0, 0, 0, 0.6);
  --f7-list-item-after-text-color: rgba(0, 0, 0, 0.5);
  --f7-list-item-footer-text-color: rgba(0, 0, 0, 0.6);
  --f7-list-button-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-list-button-hover-bg-color: rgba(0, 0, 0, 0.03);
  --f7-list-item-divider-text-color: rgba(0, 0, 0, 0.6);
  --f7-list-group-title-text-color: rgba(0, 0, 0, 0.6);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-list-item-text-text-color: rgba(255, 255, 255, 0.54);
  --f7-list-item-after-text-color: rgba(255, 255, 255, 0.54);
  --f7-list-item-footer-text-color: rgba(255, 255, 255, 0.54);
  --f7-list-item-divider-text-color: rgba(255, 255, 255, 0.6);
  --f7-list-group-title-text-color: rgba(255, 255, 255, 0.6);
  --f7-list-link-pressed-bg-color: rgba(255, 255, 255, 0.05);
  --f7-list-link-hover-bg-color: rgba(255, 255, 255, 0.03);
  --f7-list-button-pressed-bg-color: rgba(255, 255, 255, 0.05);
  --f7-list-button-hover-bg-color: rgba(255, 255, 255, 0.03);
}
.list {
  position: relative;
  z-index: 1;
  font-size: var(--f7-list-font-size);
  margin: var(--f7-list-margin-vertical) 0;
}
.list ul {
  list-style: none;
  margin: 0;
  padding: 0;
  position: relative;
  background: var(--f7-list-bg-color);
}
.list ul:before {
  content: '';
  position: absolute;
  background-color: var(--f7-list-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.list ul:after {
  content: '';
  position: absolute;
  background-color: var(--f7-list-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.list ul ul {
  padding-left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-list-in-list-padding-left));
}
.list ul ul:before,
.list ul ul:after {
  display: none !important;
}
.list li {
  position: relative;
  box-sizing: border-box;
}
.list .item-media {
  display: flex;
  flex-shrink: 0;
  flex-wrap: nowrap;
  align-items: center;
  box-sizing: border-box;
  padding-bottom: var(--f7-list-item-padding-vertical);
  padding-top: var(--f7-list-item-padding-vertical);
}
.list .item-media + .item-inner {
  margin-left: var(--f7-list-item-media-margin);
}
.list .item-media i + i,
.list .item-media i + img {
  margin-left: var(--f7-list-item-media-icons-margin);
}
.list .item-after {
  padding-left: var(--f7-list-item-after-padding);
}
.list .item-inner {
  position: relative;
  width: 100%;
  min-width: 0;
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
  align-items: center;
  align-self: stretch;
  padding-top: var(--f7-list-item-padding-vertical);
  padding-bottom: var(--f7-list-item-padding-vertical);
  min-height: var(--f7-list-item-min-height);
  padding-right: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
}
.list .item-title {
  min-width: 0;
  flex-shrink: 1;
  white-space: var(--f7-list-item-title-white-space);
  position: relative;
  overflow: hidden;
  text-overflow: ellipsis;
  max-width: 100%;
  font-size: var(--f7-list-item-title-font-size);
  font-weight: var(--f7-list-item-title-font-weight);
  color: var(--f7-list-item-title-text-color);
  line-height: var(--f7-list-item-title-line-height);
}
.list .item-after {
  white-space: nowrap;
  flex-shrink: 0;
  display: flex;
  font-size: var(--f7-list-item-after-font-size);
  font-weight: var(--f7-list-item-after-font-weight);
  color: var(--f7-list-item-after-text-color);
  line-height: var(--f7-list-item-after-line-height);
  margin-left: auto;
}
.list .item-header,
.list .item-footer {
  white-space: normal;
}
.list .item-header {
  color: var(--f7-list-item-header-text-color);
  font-size: var(--f7-list-item-header-font-size);
  font-weight: var(--f7-list-item-header-font-weight);
  line-height: var(--f7-list-item-header-line-height);
}
.list .item-footer {
  color: var(--f7-list-item-footer-text-color);
  font-size: var(--f7-list-item-footer-font-size);
  font-weight: var(--f7-list-item-footer-font-weight);
  line-height: var(--f7-list-item-footer-line-height);
}
.list .item-link,
.list .list-button {
  transition-duration: 300ms;
  transition-property: background-color;
  display: block;
  position: relative;
  overflow: hidden;
  z-index: 0;
}
.list .item-link {
  color: inherit;
}
.list .item-link.active-state {
  background-color: var(--f7-list-link-pressed-bg-color);
}
.list .item-link .item-inner {
  padding-right: calc(var(--f7-list-chevron-icon-area) + var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
}
.list .item-content {
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
  align-items: center;
  min-height: var(--f7-list-item-min-height);
  padding-left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-left));
}
.list .item-subtitle {
  position: relative;
  overflow: hidden;
  white-space: nowrap;
  max-width: 100%;
  text-overflow: ellipsis;
  font-size: var(--f7-list-item-subtitle-font-size);
  font-weight: var(--f7-list-item-subtitle-font-weight);
  color: var(--f7-list-item-subtitle-text-color);
  line-height: var(--f7-list-item-subtitle-line-height);
}
.list .item-text {
  position: relative;
  overflow: hidden;
  text-overflow: ellipsis;
  /* autoprefixer: ignore next */
  -webkit-line-clamp: var(--f7-list-item-text-max-lines);
  /* autoprefixer: ignore next */
  -webkit-box-orient: vertical;
  display: -webkit-box;
  font-size: var(--f7-list-item-text-font-size);
  font-weight: var(--f7-list-item-text-font-weight);
  color: var(--f7-list-item-text-text-color);
  line-height: var(--f7-list-item-text-line-height);
  max-height: calc(var(--f7-list-item-text-line-height) * var(--f7-list-item-text-max-lines));
}
.list .item-title-row {
  position: relative;
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
}
.list .item-title-row .item-after {
  align-self: center;
}
.list .item-row {
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
}
.list .item-cell {
  display: block;
  align-self: center;
  box-sizing: border-box;
  width: 100%;
  min-width: 0;
  margin-left: var(--f7-list-item-cell-margin);
  flex-shrink: 1;
}
.list .item-cell:first-child {
  margin-left: 0;
}
.list .ripple-wave + .item-cell {
  margin-left: 0;
}
.list li:last-child .list-button:after {
  display: none !important;
}
.list li:last-child > .item-inner:after,
.list li:last-child li:last-child > .item-inner:after,
.list li:last-child > .item-content > .item-inner:after,
.list li:last-child li:last-child > .item-content > .item-inner:after,
.list li:last-child > .swipeout-content > .item-content > .item-inner:after,
.list li:last-child li:last-child > .swipeout-content > .item-content > .item-inner:after,
.list li:last-child > .item-link > .item-content > .item-inner:after,
.list li:last-child li:last-child > .item-link > .item-content > .item-inner:after {
  display: none !important;
}
.list li li:last-child .item-inner:after,
.list li:last-child li .item-inner:after {
  content: '';
  position: absolute;
  background-color: var(--f7-list-item-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.list.no-hairlines:before,
.list.no-hairlines ul:before,
.md .list.no-hairlines-md:before,
.md .list.no-hairlines-md ul:before,
.ios .list.no-hairlines-ios:before,
.ios .list.no-hairlines-ios ul:before,
.aurora .list.no-hairlines-aurora:before,
.aurora .list.no-hairlines-aurora ul:before,
.list.no-hairlines:after,
.list.no-hairlines ul:after,
.md .list.no-hairlines-md:after,
.md .list.no-hairlines-md ul:after,
.ios .list.no-hairlines-ios:after,
.ios .list.no-hairlines-ios ul:after,
.aurora .list.no-hairlines-aurora:after,
.aurora .list.no-hairlines-aurora ul:after {
  display: none !important;
}
.list.no-hairline-top:before,
.list.no-hairline-top ul:before,
.md .list.no-hairline-top-md:before,
.md .list.no-hairline-top-md ul:before,
.ios .list.no-hairline-top-ios:before,
.ios .list.no-hairline-top-ios ul:before,
.aurora .list.no-hairline-top-aurora:before,
.aurora .list.no-hairline-top-aurora ul:before {
  display: none !important;
}
.list.no-hairline-bottom:after,
.list.no-hairline-bottom ul:after,
.md .list.no-hairline-bottom-md:after,
.md .list.no-hairline-bottom-md ul:after,
.ios .list.no-hairline-bottom-ios:after,
.ios .list.no-hairline-bottom-ios ul:after,
.aurora .list.no-hairline-bottom-aurora:after,
.aurora .list.no-hairline-bottom-aurora ul:after {
  display: none !important;
}
.list.no-hairlines-between .item-inner:after,
.md .list.no-hairlines-between-md .item-inner:after,
.ios .list.no-hairlines-between-ios .item-inner:after,
.aurora .list.no-hairlines-between-aurora .item-inner:after,
.list.no-hairlines-between .list-button:after,
.md .list.no-hairlines-between-md .list-button:after,
.ios .list.no-hairlines-between-ios .list-button:after,
.aurora .list.no-hairlines-between-aurora .list-button:after,
.list.no-hairlines-between .item-divider:after,
.md .list.no-hairlines-between-md .item-divider:after,
.ios .list.no-hairlines-between-ios .item-divider:after,
.aurora .list.no-hairlines-between-aurora .item-divider:after,
.list.no-hairlines-between .list-group-title:after,
.md .list.no-hairlines-between-md .list-group-title:after,
.ios .list.no-hairlines-between-ios .list-group-title:after,
.aurora .list.no-hairlines-between-aurora .list-group-title:after,
.list.no-hairlines-between .list-group-title:after,
.md .list.no-hairlines-between-md .list-group-title:after,
.ios .list.no-hairlines-between-ios .list-group-title:after,
.aurora .list.no-hairlines-between-aurora .list-group-title:after {
  display: none !important;
}
.list.no-hairlines-between.simple-list li:after,
.md .list.no-hairlines-between-md.simple-list li:after,
.ios .list.no-hairlines-between-ios.simple-list li:after,
.aurora .list.no-hairlines-between-aurora.simple-list li:after {
  display: none !important;
}
.list.no-hairlines-between.links-list a:after,
.md .list.no-hairlines-between-md.links-list a:after,
.ios .list.no-hairlines-between-ios.links-list a:after,
.aurora .list.no-hairlines-between-aurora.links-list a:after {
  display: none !important;
}
.list-button {
  padding: 0 var(--f7-list-item-padding-horizontal);
  line-height: var(--f7-list-item-min-height);
  color: var(--f7-list-button-text-color, var(--f7-theme-color));
  font-size: var(--f7-list-button-font-size);
  font-weight: var(--f7-list-button-font-weight);
  text-align: var(--f7-list-button-text-align);
}
.list-button:after {
  content: '';
  position: absolute;
  background-color: var(--f7-list-button-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.list-button.active-state {
  background-color: var(--f7-list-button-pressed-bg-color);
}
.list-button[class*="color-"] {
  --f7-list-button-text-color: var(--f7-theme-color);
}
.simple-list li {
  position: relative;
  white-space: nowrap;
  text-overflow: ellipsis;
  max-width: 100%;
  box-sizing: border-box;
  display: flex;
  justify-content: space-between;
  align-items: center;
  align-content: center;
  line-height: var(--f7-list-item-min-height);
  height: var(--f7-list-item-min-height);
  padding-left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
}
.simple-list li:after {
  left: var(--f7-list-item-padding-horizontal);
  width: auto;
  left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-left));
  right: 0;
}
.simple-list li:last-child:after {
  display: none !important;
}
.links-list li {
  z-index: 1;
}
.links-list a {
  transition-duration: 300ms;
  transition-property: background-color;
  display: block;
  position: relative;
  overflow: hidden;
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: space-between;
  box-sizing: border-box;
  white-space: nowrap;
  text-overflow: ellipsis;
  max-width: 100%;
  height: var(--f7-list-item-min-height);
  color: inherit;
}
.links-list a .ripple-wave {
  z-index: 0;
}
.links-list a:after {
  width: auto;
}
.links-list a.active-state {
  background-color: var(--f7-list-link-pressed-bg-color);
}
.links-list a {
  padding-left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-list-chevron-icon-area) + var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
}
.links-list a:after {
  left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-left));
  right: 0;
}
.links-list li:last-child a:after {
  display: none !important;
}
.simple-list li:after,
.links-list a:after,
.list .item-inner:after {
  content: '';
  position: absolute;
  background-color: var(--f7-list-item-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.media-list,
li.media-item {
  --f7-list-item-padding-vertical: var(--f7-list-media-item-padding-vertical);
  --f7-list-item-padding-horizontal: var(--f7-list-media-item-padding-horizontal);
}
.media-list .item-title,
li.media-item .item-title {
  font-weight: var(--f7-list-media-item-title-font-weight, var(--f7-list-item-title-font-weight, inherit));
}
.media-list .item-inner,
li.media-item .item-inner {
  display: block;
  align-self: stretch;
}
.media-list .item-media,
li.media-item .item-media {
  align-self: flex-start;
}
.media-list .item-media img,
li.media-item .item-media img {
  display: block;
}
.media-list .item-link .item-inner,
li.media-item .item-link .item-inner {
  padding-right: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
}
.media-list .item-link .item-title-row,
li.media-item .item-link .item-title-row {
  padding-right: calc(var(--f7-list-chevron-icon-area));
}
.media-list.chevron-center .item-link .item-inner,
.media-list .chevron-center .item-link .item-inner,
.media-list .item-link.chevron-center .item-inner,
li.media-item.chevron-center .item-link .item-inner,
li.media-item .item-link.chevron-center .item-inner,
li.media-item .chevron-center .item-link .item-inner {
  padding-right: calc(var(--f7-list-chevron-icon-area) + var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
}
.media-list.chevron-center .item-title-row,
.media-list .chevron-center .item-title-row,
li.media-item.chevron-center .item-title-row,
li.media-item .chevron-center .item-title-row {
  padding-right: 0;
}
.list .item-link .item-inner:before,
.links-list a:before,
.media-list .item-link .item-title-row:before,
li.media-item .item-link .item-title-row:before,
.media-list.chevron-center .item-link .item-inner:before,
.media-list .chevron-center .item-link .item-inner:before,
.media-list .item-link.chevron-center .item-inner:before,
li.media-item.chevron-center .item-link .item-inner:before,
li.media-item .chevron-center .item-link .item-inner:before,
li.media-item .item-link.chevron-center .item-inner:before {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  position: absolute;
  top: 50%;
  width: 8px;
  height: 14px;
  margin-top: -7px;
  font-size: var(--f7-list-chevron-icon-font-size);
  line-height: 14px;
  color: var(--f7-list-chevron-icon-color);
  pointer-events: none;
  right: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
  content: 'chevron_right';
}
.media-list.chevron-center .item-title-row:before,
.media-list .chevron-center .item-title-row:before,
li.media-item.chevron-center .item-title-row:before,
li.media-item .chevron-center .item-title-row:before {
  display: none;
}
.media-list .item-link .item-inner:before,
li.media-item .item-link .item-inner:before {
  display: none;
}
.media-list .item-link .item-title-row:before,
li.media-item .item-link .item-title-row:before {
  right: 0;
}
.list-group ul:after,
.list-group ul:before {
  z-index: 25 !important;
}
.list-group + .list-group ul:before {
  display: none !important;
}
li.item-divider,
.item-divider,
li.list-group-title {
  white-space: nowrap;
  position: relative;
  max-width: 100%;
  text-overflow: ellipsis;
  overflow: hidden;
  z-index: 15;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
  box-sizing: border-box;
  display: flex;
  align-items: center;
  align-content: center;
}
li.item-divider:after,
.item-divider:after,
li.list-group-title:after {
  display: none !important;
}
li.item-divider,
.item-divider {
  margin-top: -1px;
  height: var(--f7-list-item-divider-height);
  color: var(--f7-list-item-divider-text-color);
  font-size: var(--f7-list-item-divider-font-size);
  font-weight: var(--f7-list-item-divider-font-weight);
  background-color: var(--f7-list-item-divider-bg-color);
  line-height: var(--f7-list-item-divider-line-height);
}
li.item-divider:before,
.item-divider:before {
  content: '';
  position: absolute;
  background-color: var(--f7-list-item-divider-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
li.list-group-title,
.list li.list-group-title {
  position: relative;
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  margin-top: 0;
  z-index: 20;
  height: var(--f7-list-group-title-height);
  color: var(--f7-list-group-title-text-color);
  font-size: var(--f7-list-group-title-font-size);
  font-weight: var(--f7-list-group-title-font-weight);
  background-color: var(--f7-list-group-title-bg-color);
  line-height: var(--f7-list-group-title-line-height);
}
.page-with-navbar-large li.list-group-title,
.page-with-navbar-large .list li.list-group-title {
  top: calc(-1 * var(--f7-navbar-large-title-height));
}
.list.inset {
  margin-left: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-left));
  margin-right: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-right));
  border-radius: var(--f7-list-inset-border-radius);
  --f7-safe-area-left: 0px;
  --f7-safe-area-right: 0px;
}
.list.inset .block-title {
  margin-left: 0;
  margin-right: 0;
}
.list.inset ul {
  border-radius: var(--f7-list-inset-border-radius);
}
.list.inset ul:before,
.list.inset ul:after {
  display: none !important;
}
.list.inset li.swipeout:first-child,
.list.inset li:first-child > a {
  border-radius: var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius) 0 0;
}
.list.inset li.swipeout:last-child,
.list.inset li:last-child > a {
  border-radius: 0 0 var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius);
}
.list.inset li.swipeout:first-child:last-child,
.list.inset li:first-child:last-child > a {
  border-radius: var(--f7-list-inset-border-radius);
}
@media (min-width: 480px) {
  .list.xsmall-inset {
    margin-left: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-right));
    border-radius: var(--f7-list-inset-border-radius);
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .list.xsmall-inset .block-title {
    margin-left: 0;
    margin-right: 0;
  }
  .list.xsmall-inset ul {
    border-radius: var(--f7-list-inset-border-radius);
  }
  .list.xsmall-inset ul:before,
  .list.xsmall-inset ul:after {
    display: none !important;
  }
  .list.xsmall-inset li:first-child > a {
    border-radius: var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius) 0 0;
  }
  .list.xsmall-inset li:last-child > a {
    border-radius: 0 0 var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius);
  }
  .list.xsmall-inset li:first-child:last-child > a {
    border-radius: var(--f7-list-inset-border-radius);
  }
}
@media (min-width: 568px) {
  .list.small-inset {
    margin-left: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-right));
    border-radius: var(--f7-list-inset-border-radius);
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .list.small-inset .block-title {
    margin-left: 0;
    margin-right: 0;
  }
  .list.small-inset ul {
    border-radius: var(--f7-list-inset-border-radius);
  }
  .list.small-inset ul:before,
  .list.small-inset ul:after {
    display: none !important;
  }
  .list.small-inset li:first-child > a {
    border-radius: var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius) 0 0;
  }
  .list.small-inset li:last-child > a {
    border-radius: 0 0 var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius);
  }
  .list.small-inset li:first-child:last-child > a {
    border-radius: var(--f7-list-inset-border-radius);
  }
}
@media (min-width: 768px) {
  .list.medium-inset {
    margin-left: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-right));
    border-radius: var(--f7-list-inset-border-radius);
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .list.medium-inset .block-title {
    margin-left: 0;
    margin-right: 0;
  }
  .list.medium-inset ul {
    border-radius: var(--f7-list-inset-border-radius);
  }
  .list.medium-inset ul:before,
  .list.medium-inset ul:after {
    display: none !important;
  }
  .list.medium-inset li:first-child > a {
    border-radius: var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius) 0 0;
  }
  .list.medium-inset li:last-child > a {
    border-radius: 0 0 var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius);
  }
  .list.medium-inset li:first-child:last-child > a {
    border-radius: var(--f7-list-inset-border-radius);
  }
}
@media (min-width: 1024px) {
  .list.large-inset {
    margin-left: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-right));
    border-radius: var(--f7-list-inset-border-radius);
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .list.large-inset .block-title {
    margin-left: 0;
    margin-right: 0;
  }
  .list.large-inset ul {
    border-radius: var(--f7-list-inset-border-radius);
  }
  .list.large-inset ul:before,
  .list.large-inset ul:after {
    display: none !important;
  }
  .list.large-inset li:first-child > a {
    border-radius: var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius) 0 0;
  }
  .list.large-inset li:last-child > a {
    border-radius: 0 0 var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius);
  }
  .list.large-inset li:first-child:last-child > a {
    border-radius: var(--f7-list-inset-border-radius);
  }
}
@media (min-width: 1200px) {
  .list.xlarge-inset {
    margin-left: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-left));
    margin-right: calc(var(--f7-list-inset-side-margin) + var(--f7-safe-area-outer-right));
    border-radius: var(--f7-list-inset-border-radius);
    --f7-safe-area-left: 0px;
    --f7-safe-area-right: 0px;
  }
  .list.xlarge-inset .block-title {
    margin-left: 0;
    margin-right: 0;
  }
  .list.xlarge-inset ul {
    border-radius: var(--f7-list-inset-border-radius);
  }
  .list.xlarge-inset ul:before,
  .list.xlarge-inset ul:after {
    display: none !important;
  }
  .list.xlarge-inset li:first-child > a {
    border-radius: var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius) 0 0;
  }
  .list.xlarge-inset li:last-child > a {
    border-radius: 0 0 var(--f7-list-inset-border-radius) var(--f7-list-inset-border-radius);
  }
  .list.xlarge-inset li:first-child:last-child > a {
    border-radius: var(--f7-list-inset-border-radius);
  }
}
.list.no-chevron,
.list .no-chevron {
  --f7-list-chevron-icon-color: transparent;
  --f7-list-chevron-icon-area: 0px;
}
.ios .item-link.active-state .item-inner:after,
.ios .list-button.active-state:after,
.ios .links-list a.active-state:after {
  background-color: transparent;
}
.ios .links-list a.active-state,
.ios .list .item-link.active-state,
.ios .list .list-button.active-state {
  transition-duration: 0ms;
}
.md .list .item-media {
  min-width: 40px;
}
.aurora .list .item-media {
  min-width: 18px;
}
.aurora .list .item-link .item-inner:before,
.aurora .links-list a:before,
.aurora .media-list .item-link .item-title-row:before,
.aurora li.media-item .item-link .item-title-row:before,
.aurora .media-list.chevron-center .item-link .item-inner:before,
.aurora .media-list .chevron-center .item-link .item-inner:before,
.aurora .media-list .item-link.chevron-center .item-inner:before,
.aurora li.media-item.chevron-center .item-link .item-inner:before,
.aurora li.media-item .chevron-center .item-link .item-inner:before,
.aurora li.media-item .item-link.chevron-center .item-inner:before {
  content: 'chevron_right_aurora';
}
.aurora .links-list a,
.aurora .list .item-link,
.aurora .list .list-button {
  transition-duration: 0ms;
}
.aurora.device-desktop .links-list a:hover:not(.active-state):not(.no-hover),
.aurora.device-desktop .list .item-link:hover:not(.active-state):not(.no-hover) {
  background: var(--f7-list-link-hover-bg-color);
}
.aurora.device-desktop .list .list-button:hover:not(.active-state):not(.no-hover) {
  background: var(--f7-list-button-hover-bg-color);
}
/* === Badge === */
:root {
  --f7-badge-text-color: #fff;
  --f7-badge-bg-color: #8e8e93;
  --f7-badge-padding: 0 4px;
  --f7-badge-in-icon-size: 16px;
  --f7-badge-in-icon-font-size: 10px;
  --f7-badge-font-weight: normal;
  --f7-badge-font-size: 12px;
}
.ios {
  --f7-badge-size: 20px;
}
.md {
  --f7-badge-size: 18px;
}
.aurora {
  --f7-badge-size: 18px;
  --f7-badge-font-weight: 600;
  --f7-badge-in-icon-size: 15px;
}
.badge {
  display: inline-flex;
  align-items: center;
  align-content: center;
  justify-content: center;
  color: var(--f7-badge-text-color);
  background: var(--f7-badge-bg-color);
  position: relative;
  box-sizing: border-box;
  text-align: center;
  vertical-align: middle;
  font-weight: var(--f7-badge-font-weight);
  font-size: var(--f7-badge-font-size);
  border-radius: var(--f7-badge-size);
  padding: var(--f7-badge-padding);
  height: var(--f7-badge-size);
  min-width: var(--f7-badge-size);
}
.icon .badge,
.f7-icons .badge,
.framework7-icons .badge,
.material-icons .badge {
  position: absolute;
  left: 100%;
  margin-left: -10px;
  top: -2px;
  font-family: var(--f7-font-family);
  --f7-badge-font-size: var(--f7-badge-in-icon-font-size);
  --f7-badge-size: var(--f7-badge-in-icon-size);
}
.badge[class*="color-"] {
  --f7-badge-bg-color: var(--f7-theme-color);
}
:root {
  --f7-button-min-width: 32px;
  --f7-button-bg-color: transparent;
  --f7-button-border-width: 0px;
  /*
  --f7-button-text-color: var(--f7-theme-color);
  --f7-button-pressed-text-color: var(--f7-button-text-color, var(--f7-theme-color));
  --f7-button-border-color: var(--f7-theme-color);
  --f7-button-fill-text-color: #fff;
  --f7-button-fill-bg-color: var(--f7-theme-color);
  --f7-button-outline-border-color: var(--f7-theme-color);
  */
  --f7-button-outline-border-width: 2px;
  --f7-button-raised-box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0,0,0,0.24);
  --f7-button-raised-pressed-box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0,0,0,0.23);
  --f7-segmented-raised-divider-color: rgba(0, 0, 0, 0.1);
  --f7-segmented-strong-padding: 2px;
  --f7-segmented-strong-between-buttons: 4px;
  --f7-segmented-strong-button-font-weight: 500;
  --f7-segmented-strong-button-active-box-shadow: 0px 2px 2px rgba(0, 0, 0, 0.25);
  --f7-segmented-strong-bg-color: rgba(0, 0, 0, 0.07);
  --f7-segmented-strong-button-text-color: #000;
  --f7-segmented-strong-button-pressed-bg-color: rgba(0, 0, 0, 0.07);
  --f7-segmented-strong-button-hover-bg-color: rgba(0, 0, 0, 0.04);
  --f7-segmented-strong-button-active-text-color: #000;
  --f7-segmented-strong-button-active-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-segmented-strong-bg-color: rgba(255, 255, 255, 0.1);
  --f7-segmented-strong-button-pressed-bg-color: rgba(255, 255, 255, 0.04);
  --f7-segmented-strong-button-hover-bg-color: rgba(255, 255, 255, 0.02);
  --f7-segmented-strong-button-active-bg-color: rgba(255, 255, 255, 0.14);
  --f7-segmented-strong-button-text-color: #fff;
  --f7-segmented-strong-button-active-text-color: #fff;
}
.ios {
  --f7-button-font-size: 13px;
  --f7-button-height: 28px;
  --f7-button-padding-horizontal: 10px;
  --f7-button-border-radius: 5px;
  --f7-button-font-weight: 600;
  --f7-button-letter-spacing: 0;
  --f7-button-text-transform: uppercase;
  /*
  --f7-button-pressed-bg-color: rgba(var(--f7-theme-color-rgb), .15);
  --f7-button-fill-pressed-bg-color: var(--f7-theme-color-tint);
  */
  --f7-button-large-height: 44px;
  --f7-button-large-font-size: 17px;
  --f7-button-large-font-weight: 500;
  --f7-button-large-text-transform: none;
  --f7-button-small-height: 26px;
  --f7-button-small-font-size: 13px;
  --f7-button-small-font-weight: 600;
  --f7-button-small-text-transform: uppercase;
  --f7-button-small-outline-border-width: 2px;
  --f7-segmented-strong-button-text-transform: none;
  --f7-segmented-strong-button-active-font-weight: 600;
}
.md {
  --f7-button-font-size: 14px;
  --f7-button-height: 36px;
  --f7-button-padding-horizontal: 8px;
  --f7-button-border-radius: 4px;
  --f7-button-font-weight: 500;
  --f7-button-letter-spacing: 0.03em;
  --f7-button-text-transform: uppercase;
  /*
  --f7-button-fill-pressed-bg-color: var(--f7-theme-color-shade);
  */
  --f7-button-large-height: 48px;
  --f7-button-large-font-size: 14px;
  --f7-button-large-font-weight: 500;
  --f7-button-large-text-transform: uppercase;
  --f7-button-small-height: 28px;
  --f7-button-small-font-size: 12px;
  --f7-button-small-font-weight: 500;
  --f7-button-small-text-transform: uppercase;
  --f7-button-small-outline-border-width: 2px;
  --f7-segmented-strong-button-text-transform: uppercase;
  --f7-segmented-strong-button-active-font-weight: 500;
  --f7-button-pressed-bg-color: rgba(0, 0, 0, 0.1);
}
.md .theme-dark,
.md.theme-dark {
  --f7-button-pressed-bg-color: rgba(255, 255, 255, 0.1);
}
.aurora {
  /*
  --f7-button-hover-bg-color: rgba(var(--f7-theme-color-rgb), .07);
  --f7-button-fill-hover-bg-color: var(--f7-theme-color-tint);
  */
  --f7-button-font-size: 14px;
  --f7-button-height: 28px;
  --f7-button-min-width: 24px;
  --f7-button-padding-horizontal: 10px;
  --f7-button-border-radius: 4px;
  --f7-button-font-weight: 500;
  --f7-button-letter-spacing: 0.02;
  --f7-button-text-transform: none;
  /*
  --f7-button-pressed-bg-color: rgba(var(--f7-theme-color-rgb), .15);
  --f7-button-fill-pressed-bg-color: var(--f7-theme-color-shade);
  */
  --f7-button-large-height: 34px;
  --f7-button-large-font-size: 14px;
  --f7-button-large-font-weight: 600;
  --f7-button-large-text-transform: none;
  --f7-button-small-height: 24px;
  --f7-button-small-font-size: 12px;
  --f7-button-small-font-weight: 600;
  --f7-button-small-text-transform: none;
  --f7-button-small-outline-border-width: 1px;
  --f7-segmented-strong-button-text-transform: none;
  --f7-segmented-strong-button-active-font-weight: 600;
}
button {
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  width: 100%;
}
.button {
  text-decoration: none;
  text-align: center;
  display: block;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  background: none;
  margin: 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  position: relative;
  overflow: hidden;
  font-family: inherit;
  cursor: pointer;
  outline: 0;
  box-sizing: border-box;
  vertical-align: middle;
  justify-content: center;
  align-items: center;
  border: var(--f7-button-border-width, 0px) solid var(--f7-button-border-color, var(--f7-theme-color));
  font-size: var(--f7-button-font-size);
  color: var(--f7-button-text-color, var(--f7-theme-color));
  height: var(--f7-button-height);
  line-height: calc(var(--f7-button-height) - var(--f7-button-border-width, 0) * 2);
  padding: var(--f7-button-padding-vertical, 0px) var(--f7-button-padding-horizontal);
  border-radius: var(--f7-button-border-radius);
  min-width: var(--f7-button-min-width);
  font-weight: var(--f7-button-font-weight);
  letter-spacing: var(--f7-button-letter-spacing);
  text-transform: var(--f7-button-text-transform);
  background-color: var(--f7-button-bg-color);
  box-shadow: var(--f7-button-box-shadow);
}
.button.active-state {
  background-color: var(--f7-button-pressed-bg-color, rgba(var(--f7-theme-color-rgb), 0.15));
  color: var(--f7-button-pressed-text-color, var(--f7-button-text-color, var(--f7-theme-color)));
}
input[type="submit"].button,
input[type="button"].button {
  width: 100%;
}
.button > i + span,
.button > span + span,
.button > span + i,
.button > i + i {
  margin-left: 4px;
}
.subnavbar .button,
.navbar .button,
.toolbar .button,
.searchbar .button,
.appbar .button {
  color: var(--f7-button-text-color, var(--f7-theme-color));
}
.button-round,
.ios .button-round-ios,
.md .button-round-md,
.aurora .button-round-aurora {
  --f7-button-border-radius: var(--f7-button-height);
}
.button-fill,
.ios .button-fill-ios,
.md .button-fill-md,
.aurora .button-fill-aurora,
.button-active,
.button.tab-link-active {
  --f7-button-bg-color: var(--f7-button-fill-bg-color, var(--f7-theme-color));
  --f7-button-text-color: var(--f7-button-fill-text-color, #fff);
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
}
.button-fill,
.ios .button-fill-ios,
.md .button-fill-md,
.aurora .button-fill-aurora {
  --f7-button-pressed-bg-color: var(--f7-button-fill-pressed-bg-color);
}
.button-active,
.button.tab-link-active {
  --f7-button-pressed-bg-color: var(--f7-button-bg-color);
}
.button-outline,
.ios .button-outline-ios,
.md .button-outline-md,
.aurora .button-outline-aurora {
  --f7-button-border-color: var(--f7-button-outline-border-color, var(--f7-theme-color));
  --f7-button-border-width: var(--f7-button-outline-border-width);
}
.button-large,
.ios .button-large-ios,
.md .button-large-md,
.aurora .button-large-aurora {
  --f7-button-height: var(--f7-button-large-height);
  --f7-button-font-size: var(--f7-button-large-font-size);
  --f7-button-font-weight: var(--f7-button-large-font-weight);
  --f7-button-text-transform: var(--f7-button-large-text-transform);
}
.button-small,
.ios .button-small-ios,
.md .button-small-md,
.aurora .button-small-aurora {
  --f7-button-outline-border-width: var(--f7-button-small-outline-border-width);
  --f7-button-height: var(--f7-button-small-height);
  --f7-button-font-size: var(--f7-button-small-font-size);
  --f7-button-font-weight: var(--f7-button-small-font-weight);
  --f7-button-text-transform: var(--f7-button-small-text-transform);
}
.ios .button-small.button-fill,
.ios .button-small-ios.button-fill,
.ios .button-small.button-fill-ios {
  --f7-button-border-width: var(--f7-button-small-outline-border-width);
  --f7-button-pressed-text-color: var(--f7-theme-color);
  --f7-button-pressed-bg-color: transparent;
}
.segmented {
  align-self: center;
  display: flex;
  flex-wrap: nowrap;
  border-radius: var(--f7-button-border-radius);
  box-shadow: var(--f7-button-box-shadow);
  box-sizing: border-box;
}
.segmented .button,
.segmented button {
  width: 100%;
  flex-shrink: 1;
  min-width: 0;
  border-radius: 0;
}
.segmented .button:first-child {
  border-radius: var(--f7-button-border-radius) 0 0 var(--f7-button-border-radius);
}
.segmented .button:not(.button-outline):first-child {
  border-left: none;
}
.segmented .button.button-outline:nth-child(n + 2) {
  border-left: none;
}
.segmented .button:last-child {
  border-radius: 0 var(--f7-button-border-radius) var(--f7-button-border-radius) 0;
}
.segmented .button-round:first-child {
  border-radius: var(--f7-button-height) 0 0 var(--f7-button-height);
}
.segmented .button-round:last-child {
  border-radius: 0 var(--f7-button-height) var(--f7-button-height) 0;
}
.segmented .button:first-child:last-child {
  border-radius: var(--f7-button-border-radius);
}
.segmented-raised,
.ios .segmented-raised-ios,
.md .segmented-raised-md,
.aurora .segmented-raised-aurora {
  box-shadow: var(--f7-button-raised-box-shadow);
}
.segmented-raised .button:not(.button-outline),
.ios .segmented-raised-ios .button:not(.button-outline),
.md .segmented-raised-md .button:not(.button-outline),
.aurora .segmented-raised-aurora .button:not(.button-outline) {
  border-left: 1px solid var(--f7-segmented-raised-divider-color);
}
.button-raised,
.ios .button-raised-ios,
.md .button-raised-md,
.aurora .button-raised-aurora {
  --f7-button-box-shadow: var(--f7-button-raised-box-shadow);
}
.button-raised.active-state,
.ios .button-raised-ios.active-state,
.md .button-raised-md.active-state,
.aurora .button-raised-aurora.active-state {
  --f7-button-box-shadow: var(--f7-button-raised-pressed-box-shadow);
}
.segmented-strong,
.ios .segmented-strong-ios,
.md .segmented-strong-md,
.aurora .segmented-strong-aurora {
  --f7-button-bg-color: transparent;
  --f7-button-hover-bg-color: var(--f7-segmented-strong-button-hover-bg-color);
  --f7-button-text-color: var(--f7-segmented-strong-button-text-color);
  --f7-button-font-weight: var(--f7-segmented-strong-button-font-weight);
  --f7-button-text-transform: var(--f7-segmented-strong-button-text-transform);
  --f7-button-pressed-bg-color: var(--f7-segmented-strong-button-pressed-bg-color);
  background: var(--f7-segmented-strong-bg-color);
  border-radius: calc(var(--f7-button-border-radius) + 2px);
  box-shadow: none;
  padding: var(--f7-segmented-strong-padding);
  overflow: hidden;
}
.segmented-strong .button,
.ios .segmented-strong-ios .button,
.md .segmented-strong-md .button,
.aurora .segmented-strong-aurora .button,
.segmented-strong .button:first-child,
.ios .segmented-strong-ios .button:first-child,
.md .segmented-strong-md .button:first-child,
.aurora .segmented-strong-aurora .button:first-child,
.segmented-strong .button:last-child,
.ios .segmented-strong-ios .button:last-child,
.md .segmented-strong-md .button:last-child,
.aurora .segmented-strong-aurora .button:last-child {
  border-radius: var(--f7-button-border-radius);
}
.segmented-strong .button + .button,
.ios .segmented-strong-ios .button + .button,
.md .segmented-strong-md .button + .button,
.aurora .segmented-strong-aurora .button + .button {
  margin-left: var(--f7-segmented-strong-between-buttons);
}
.segmented-strong .button.button-active,
.ios .segmented-strong-ios .button.button-active,
.md .segmented-strong-md .button.button-active,
.aurora .segmented-strong-aurora .button.button-active,
.segmented-strong .button.tab-link-active,
.ios .segmented-strong-ios .button.tab-link-active,
.md .segmented-strong-md .button.tab-link-active,
.aurora .segmented-strong-aurora .button.tab-link-active {
  --f7-button-hover-bg-color: var(--f7-segmented-strong-button-active-bg-color);
  --f7-button-bg-color: var(--f7-segmented-strong-button-active-bg-color);
  --f7-button-text-color: var(--f7-segmented-strong-button-active-text-color);
  --f7-button-font-weight: var(--f7-segmented-strong-button-active-font-weight);
  --f7-button-box-shadow: var(--f7-segmented-strong-button-active-box-shadow);
}
.segmented-round,
.ios .segmented-round-ios,
.md .segmented-round-md,
.aurora .segmented-round-aurora {
  border-radius: var(--f7-button-height);
}
.subnavbar .segmented {
  width: 100%;
}
.ios .button {
  transition-duration: 100ms;
}
.ios .button-fill,
.ios .button-fill-ios {
  --f7-button-pressed-bg-color: var(--f7-button-fill-pressed-bg-color, var(--f7-theme-color-tint));
}
.ios .button-small,
.ios .button-small-ios {
  transition-duration: 200ms;
}
.md .button {
  transition-duration: 300ms;
  transform: translate3d(0, 0, 0);
}
.md .button-fill,
.md .button-fill-md {
  --f7-button-pressed-bg-color: var(--f7-button-fill-pressed-bg-color, var(--f7-theme-color-shade));
}
.aurora .button {
  transition-duration: 100ms;
  transform: translate3d(0, 0, 0);
}
.aurora.device-desktop .button:not(.active-state):not(.no-hover):hover {
  background-color: var(--f7-button-hover-bg-color, rgba(var(--f7-theme-color-rgb), 0.07));
}
.aurora .button-fill,
.aurora .button-fill-aurora {
  --f7-button-pressed-bg-color: var(--f7-button-fill-pressed-bg-color, var(--f7-theme-color-shade));
}
.aurora .button-fill,
.aurora .button-active,
.aurora .button.tab-link-active,
.aurora .button-fill-aurora {
  --f7-button-hover-bg-color: var(--f7-button-fill-hover-bg-color, var(--f7-theme-color-tint));
}
/* === Touch Ripple === */
:root {
  --f7-touch-ripple-black: rgba(0, 0, 0, 0.1);
  --f7-touch-ripple-white: rgba(255, 255, 255, 0.3);
  --f7-touch-ripple-color: var(--f7-touch-ripple-black);
}
.theme-dark {
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
}
.ripple,
.fab a,
.link,
.item-link,
.list-button,
.button,
.dialog-button,
.tab-link,
.radio,
.checkbox,
.actions-button,
.speed-dial-buttons a {
  -webkit-user-select: none;
  -moz-user-select: none;
       user-select: none;
}
.ripple-wave {
  left: 0;
  top: 0;
  position: absolute !important;
  border-radius: 50%;
  pointer-events: none;
  z-index: -1;
  padding: 0;
  margin: 0;
  font-size: 0;
  transform: translate3d(0px, 0px, 0) scale(0);
  transition-duration: 1400ms;
  background-color: var(--f7-touch-ripple-color);
}
.ripple-wave.ripple-wave-fill {
  transition-duration: 300ms;
  opacity: 0.35;
}
.ripple-wave.ripple-wave-out {
  transition-duration: 600ms;
  opacity: 0;
}
.button-fill .ripple-wave,
.picker-calendar-day .ripple-wave,
.menu .ripple-wave {
  z-index: 1;
}
.checkbox .ripple-wave,
.radio .ripple-wave,
.data-table .sortable-cell .ripple-wave {
  z-index: 0;
}
[class*="ripple-color-"] {
  --f7-touch-ripple-color: var(--f7-theme-color-ripple-color);
}
/* === Icon === */
.f7-icons,
.material-icons {
  width: 1em;
  height: 1em;
}
i.icon {
  display: inline-block;
  vertical-align: middle;
  background-size: 100% auto;
  background-position: center;
  background-repeat: no-repeat;
  font-style: normal;
  position: relative;
}
.icon-back:after,
.icon-prev:after,
.icon-forward:after,
.icon-next:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
}
.icon[class*="color-"] {
  color: var(--f7-theme-color);
}
.ios .icon-back,
.ios .icon-prev,
.ios .icon-forward,
.ios .icon-next {
  width: 12px;
  height: 20px;
  line-height: 20px;
}
.ios .icon-back:after,
.ios .icon-prev:after,
.ios .icon-forward:after,
.ios .icon-next:after {
  line-height: inherit;
}
.ios .icon-prev:after,
.ios .icon-next:after {
  font-size: 16px;
}
.ios .icon-back:after,
.ios .icon-prev:after {
  content: 'chevron_left_ios';
}
.ios .icon-forward:after,
.ios .icon-next:after {
  content: 'chevron_right_ios';
}
.md .icon-back,
.md .icon-forward,
.md .icon-next,
.md .icon-prev {
  width: 24px;
  height: 24px;
}
.md .icon-back:after,
.md .icon-forward:after,
.md .icon-next:after,
.md .icon-prev:after {
  line-height: 1.2;
}
.md .icon-back:after {
  content: 'arrow_left_md';
}
.md .icon-forward:after {
  content: 'arrow_right_md';
}
.md .icon-next:after {
  content: 'chevron_right_md';
}
.md .icon-prev:after {
  content: 'chevron_left_md';
}
.aurora .f7-icons,
.aurora .material-icons {
  font-size: 18px;
}
.aurora .icon-back,
.aurora .icon-prev,
.aurora .icon-forward,
.aurora .icon-next {
  width: 9px;
  height: 14px;
  line-height: 14px;
}
.aurora .icon-back:after,
.aurora .icon-prev:after,
.aurora .icon-forward:after,
.aurora .icon-next:after {
  line-height: inherit;
}
.aurora .icon-back:after,
.aurora .icon-prev:after {
  content: 'chevron_left_aurora';
}
.aurora .icon-forward:after,
.aurora .icon-next:after {
  content: 'chevron_right_aurora';
}
.custom-modal-backdrop {
  z-index: 10500;
}
.custom-modal-backdrop,
.actions-backdrop,
.dialog-backdrop,
.popover-backdrop,
.popup-backdrop,
.preloader-backdrop,
.sheet-backdrop {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.4);
  z-index: 13000;
  visibility: hidden;
  opacity: 0;
  transition-duration: 400ms;
}
.custom-modal-backdrop.not-animated,
.actions-backdrop.not-animated,
.dialog-backdrop.not-animated,
.popover-backdrop.not-animated,
.popup-backdrop.not-animated,
.preloader-backdrop.not-animated,
.sheet-backdrop.not-animated {
  transition-duration: 0ms;
}
.custom-modal-backdrop.backdrop-in,
.actions-backdrop.backdrop-in,
.dialog-backdrop.backdrop-in,
.popover-backdrop.backdrop-in,
.popup-backdrop.backdrop-in,
.preloader-backdrop.backdrop-in,
.sheet-backdrop.backdrop-in {
  visibility: visible;
  opacity: 1;
}
/* === Appbar === */
:root {
  /*
  --f7-appbar-offset: var(--f7-appbar-height);
  --f7-appbar-extra-offset: 0px;
  --f7-appbar-bg-color: var(--f7-bars-bg-color);
  --f7-appbar-bg-color-rgb: var(--f7-bars-bg-color-rgb);
  --f7-appbar-bg-image: var(--f7-bars-bg-image);
  --f7-appbar-border-color: var(--f7-bars-border-color);
  --f7-appbar-link-color: var(--f7-bars-link-color);
  --f7-appbar-text-color: var(--f7-bars-text-color);
  */
  --f7-appbar-shadow-image: none;
}
.ios {
  --f7-appbar-height: 44px;
  --f7-appbar-inner-padding-left: 8px;
  --f7-appbar-inner-padding-right: 8px;
}
.md {
  --f7-appbar-height: 48px;
  --f7-appbar-inner-padding-left: 16px;
  --f7-appbar-inner-padding-right: 16px;
}
.aurora {
  --f7-appbar-height: 38px;
  --f7-appbar-inner-padding-left: 16px;
  --f7-appbar-inner-padding-right: 16px;
}
.appbar {
  position: relative;
  left: 0;
  top: 0;
  width: 100%;
  z-index: 500;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  box-sizing: border-box;
  margin: 0;
  transform: translate3d(0, 0, 0);
  height: calc(var(--f7-appbar-height) + var(--f7-safe-area-top));
  background-image: var(--f7-appbar-bg-image, var(--f7-bars-bg-image));
  background-color: var(--f7-appbar-bg-color, var(--f7-bars-bg-color));
  color: var(--f7-appbar-text-color, var(--f7-bars-text-color));
  font-size: var(--f7-appbar-font-size);
  z-index: 7000;
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .appbar {
    background-color: rgba(var(--f7-appbar-bg-color-rgb, var(--f7-bars-bg-color-rgb)), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.appbar .panel ~ .appbar {
  z-index: 5500;
}
.appbar a {
  color: var(--f7-appbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.appbar a.link {
  display: flex;
  justify-content: flex-start;
  line-height: var(--f7-appbar-link-line-height, var(--f7-appbar-height));
  height: var(--f7-appbar-link-height, var(--f7-appbar-height));
}
.appbar .left,
.appbar .center,
.appbar .right {
  display: flex;
  align-items: center;
}
.appbar.no-hairline:after,
.appbar.no-border:after {
  display: none !important;
}
.appbar.no-hairline .title-large:after,
.appbar.no-border .title-large:after {
  display: none !important;
}
.appbar.no-shadow:before {
  display: none !important;
}
.appbar:after,
.appbar:before {
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.appbar:after {
  content: '';
  position: absolute;
  background-color: var(--f7-appbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.appbar:before {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  top: 100%;
  bottom: auto;
  height: 8px;
  pointer-events: none;
  background: var(--f7-appbar-shadow-image);
}
.appbar:after {
  z-index: 1;
}
.appbar ~ * {
  --f7-appbar-app-offset: calc(var(--f7-appbar-height) + var(--f7-appbar-extra-offset, 0px) + var(--f7-safe-area-top));
}
.appbar ~ .views,
.appbar ~ .view,
.appbar ~ .appbar {
  --f7-safe-area-top: 0px;
}
.appbar ~ .panel .view,
.appbar ~ .panel .page,
.appbar ~ .panel .page-content {
  --f7-safe-area-top: 0px;
}
.appbar-inner {
  position: absolute;
  left: 0;
  top: var(--f7-safe-area-top);
  width: 100%;
  height: var(--f7-appbar-height);
  display: flex;
  align-items: center;
  justify-content: space-between;
  box-sizing: border-box;
  padding: 0 calc(var(--f7-appbar-inner-padding-right) + var(--f7-safe-area-right)) 0 calc(var(--f7-appbar-inner-padding-left) + var(--f7-safe-area-left));
}
.appbar-inner.stacked {
  display: none;
}
/* === Dialog === */
:root {
  --f7-dialog-button-text-color: var(--f7-theme-color);
  --f7-dialog-button-text-align: center;
  --f7-dialog-input-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-dialog-text-color: #fff;
}
.ios {
  --f7-dialog-box-shadow: none;
  --f7-dialog-width: 270px;
  --f7-dialog-inner-padding: 16px;
  --f7-dialog-border-radius: 13px;
  --f7-dialog-text-align: center;
  --f7-dialog-font-size: 14px;
  --f7-dialog-title-text-color: inherit;
  --f7-dialog-title-font-size: 18px;
  --f7-dialog-title-font-weight: 600;
  --f7-dialog-title-line-height: inherit;
  --f7-dialog-button-font-size: 17px;
  --f7-dialog-button-height: 44px;
  --f7-dialog-button-letter-spacing: 0;
  --f7-dialog-button-font-weight: 400;
  --f7-dialog-button-text-transform: none;
  --f7-dialog-input-border-radius: 4px;
  --f7-dialog-input-font-size: 14px;
  --f7-dialog-input-height: 32px;
  --f7-dialog-input-border-width: 1px;
  --f7-dialog-input-placeholder-color: #a9a9a9;
  --f7-dialog-preloader-size: 34px;
  --f7-dialog-bg-color: rgba(255, 255, 255, 0.95);
  --f7-dialog-bg-color-rgb: 255, 255, 255;
  --f7-dialog-text-color: #000;
  --f7-dialog-button-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-dialog-input-border-color: rgba(0, 0, 0, 0.3);
  --f7-dialog-border-divider-color: rgba(0, 0, 0, 0.2);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-dialog-bg-color: rgba(45, 45, 45, 0.95);
  --f7-dialog-bg-color-rgb: 45, 45, 45;
  --f7-dialog-button-pressed-bg-color: rgba(0, 0, 0, 0.2);
  --f7-dialog-border-divider-color: rgba(255, 255, 255, 0.15);
  --f7-dialog-input-border-color: rgba(255, 255, 255, 0.15);
  --f7-dialog-input-bg-color: rgba(0, 0, 0, 0.5);
}
.md {
  --f7-dialog-box-shadow: var(--f7-elevation-24);
  --f7-dialog-width: 280px;
  --f7-dialog-inner-padding: 24px;
  --f7-dialog-border-radius: 4px;
  --f7-dialog-text-align: left;
  --f7-dialog-font-size: 16px;
  --f7-dialog-title-font-size: 20px;
  --f7-dialog-title-font-weight: 500;
  --f7-dialog-title-line-height: 1.3;
  --f7-dialog-button-font-size: 14px;
  --f7-dialog-button-height: 36px;
  --f7-dialog-button-letter-spacing: 0.03em;
  --f7-dialog-button-font-weight: 500;
  --f7-dialog-button-text-transform: uppercase;
  --f7-dialog-input-border-radius: 0px;
  --f7-dialog-input-font-size: 16px;
  --f7-dialog-input-height: 36px;
  --f7-dialog-input-border-color: transparent;
  --f7-dialog-input-border-width: 0px;
  --f7-dialog-preloader-size: 32px;
  --f7-dialog-bg-color: #fff;
  --f7-dialog-text-color: rgba(0, 0, 0, 0.54);
  --f7-dialog-title-text-color: #212121;
  --f7-dialog-button-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-dialog-input-placeholder-color: rgba(0, 0, 0, 0.35);
}
.md .theme-dark,
.md.theme-dark {
  --f7-dialog-bg-color: #1c1c1d;
  --f7-dialog-title-text-color: #fff;
  --f7-dialog-button-pressed-bg-color: rgba(255, 255, 255, 0.1);
  --f7-dialog-input-bg-color: transparent;
  --f7-dialog-input-placeholder-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-dialog-box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.15), 0 25px 30px 0 rgba(0,0,0,0.35);
  --f7-dialog-width: 300px;
  --f7-dialog-inner-padding: 20px;
  --f7-dialog-border-radius: 4px;
  --f7-dialog-text-align: left;
  --f7-dialog-font-size: 14px;
  --f7-dialog-title-font-size: 14px;
  --f7-dialog-title-font-weight: 700;
  --f7-dialog-title-line-height: inherit;
  --f7-dialog-button-font-size: 13px;
  --f7-dialog-button-height: 28px;
  --f7-dialog-button-letter-spacing: 0;
  --f7-dialog-button-font-weight: 500;
  --f7-dialog-button-text-transform: none;
  /*
  --f7-dialog-button-pressed-bg-color: var(--f7-theme-color-shade);
  */
  --f7-dialog-input-border-radius: 4px;
  --f7-dialog-input-font-size: 13px;
  --f7-dialog-input-height: 24px;
  --f7-dialog-input-border-width: 1px;
  --f7-dialog-preloader-size: 24px;
  --f7-dialog-bg-color: #fff;
  --f7-dialog-title-text-color: inherit;
  --f7-dialog-text-color: #000;
  --f7-dialog-button-text-color: #fff;
  --f7-dialog-input-border-color: rgba(0, 0, 0, 0.12);
  --f7-dialog-input-placeholder-color: rgba(0, 0, 0, 0.32);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-dialog-bg-color: #1c1c1d;
  --f7-dialog-title-text-color: #fff;
  --f7-dialog-input-bg-color: rgba(0, 0, 0, 0.25);
  --f7-dialog-input-placeholder-color: rgba(255, 255, 255, 0.54);
  --f7-dialog-input-border-color: rgba(255, 255, 255, 0.15);
}
.dialog {
  position: absolute;
  z-index: 13500;
  left: 50%;
  margin-top: 0;
  top: 50%;
  overflow: hidden;
  opacity: 0;
  transform: translate3d(0, -50%, 0) scale(1.185);
  transition-property: transform, opacity;
  display: none;
  transition-duration: 400ms;
  box-shadow: var(--f7-dialog-box-shadow);
  width: var(--f7-dialog-width);
  margin-left: calc(-1 * var(--f7-dialog-width) / 2);
  border-radius: var(--f7-dialog-border-radius);
  text-align: var(--f7-dialog-text-align);
  color: var(--f7-dialog-text-color);
  font-size: var(--f7-dialog-font-size);
  background: var(--f7-dialog-bg-color);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-modals .dialog {
    background-color: rgba(var(--f7-dialog-bg-color-rgb), 0.8);
    -webkit-backdrop-filter: saturate(180%) blur(20px);
            backdrop-filter: saturate(180%) blur(20px);
  }
}
.dialog.modal-in {
  opacity: 1;
  transform: translate3d(0, -50%, 0) scale(1);
}
.dialog.modal-out {
  opacity: 0;
  z-index: 13499;
}
.dialog.not-animated {
  transition-duration: 0ms;
}
.dialog-inner {
  position: relative;
  padding: var(--f7-dialog-inner-padding);
}
.dialog-title {
  color: var(--f7-dialog-title-text-color);
  font-size: var(--f7-dialog-title-font-size);
  font-weight: var(--f7-dialog-title-font-weight);
  line-height: var(--f7-dialog-title-line-height);
}
.dialog-buttons {
  position: relative;
  display: flex;
}
.dialog-buttons-vertical .dialog-buttons {
  display: block;
  height: auto !important;
}
.dialog-button {
  box-sizing: border-box;
  overflow: hidden;
  position: relative;
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--f7-dialog-button-text-color);
  font-size: var(--f7-dialog-button-font-size);
  height: var(--f7-dialog-button-height);
  line-height: var(--f7-dialog-button-height);
  letter-spacing: var(--f7-dialog-button-letter-spacing);
  text-align: var(--f7-dialog-button-text-align);
  font-weight: var(--f7-dialog-button-font-weight);
  text-transform: var(--f7-dialog-button-text-transform);
  display: block;
  cursor: pointer;
}
.dialog-button.active-state {
  background-color: var(--f7-dialog-button-pressed-bg-color);
}
.dialog-no-buttons .dialog-buttons {
  display: none;
}
.dialog-input-field {
  position: relative;
}
input.dialog-input[type] {
  box-sizing: border-box;
  margin: 0;
  margin-top: 15px;
  border-radius: var(--f7-dialog-input-border-radius);
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  width: 100%;
  display: block;
  font-family: inherit;
  box-shadow: none;
  font-size: var(--f7-dialog-input-font-size);
  height: var(--f7-dialog-input-height);
  background-color: var(--f7-dialog-input-bg-color);
  border: var(--f7-dialog-input-border-width) solid var(--f7-dialog-input-border-color);
}
input.dialog-input[type]::-webkit-input-placeholder {
  color: var(--f7-dialog-input-placeholder-color);
}
input.dialog-input[type]::-moz-placeholder {
  color: var(--f7-dialog-input-placeholder-color);
}
input.dialog-input[type]::placeholder {
  color: var(--f7-dialog-input-placeholder-color);
}
.dialog-input-double input.dialog-input {
  border-radius: var(--f7-dialog-input-border-radius) var(--f7-dialog-input-border-radius) 0 0;
}
.dialog-input-double + .dialog-input-double input.dialog-input {
  border-radius: 0 0 var(--f7-dialog-input-border-radius) var(--f7-dialog-input-border-radius);
}
.dialog-preloader .preloader {
  --f7-preloader-size: var(--f7-dialog-preloader-size);
}
html.with-modal-dialog .page-content {
  overflow: hidden;
  -webkit-overflow-scrolling: auto;
}
.ios .dialog.modal-out {
  transform: translate3d(0, -50%, 0) scale(1);
}
.ios .dialog-inner {
  border-radius: var(--f7-dialog-border-radius) var(--f7-dialog-border-radius) 0 0;
}
.ios .dialog-inner:after {
  content: '';
  position: absolute;
  background-color: var(--f7-dialog-border-divider-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.ios .dialog-title + .dialog-text {
  margin-top: 5px;
}
.ios .dialog-buttons {
  height: 44px;
  justify-content: center;
}
.ios .dialog-button {
  width: 100%;
  padding: 0 5px;
  -webkit-box-flex: 1;
  -ms-flex: 1;
}
.ios .dialog-button:after {
  content: '';
  position: absolute;
  background-color: var(--f7-dialog-border-divider-color);
  display: block;
  z-index: 15;
  top: 0;
  right: 0;
  bottom: auto;
  left: auto;
  width: 1px;
  height: 100%;
  transform-origin: 100% 50%;
  transform: scaleX(calc(1 / var(--f7-device-pixel-ratio)));
}
.ios .dialog-button:first-child {
  border-radius: 0 0 0 var(--f7-dialog-border-radius);
}
.ios .dialog-button:last-child {
  border-radius: 0 0 var(--f7-dialog-border-radius) 0;
}
.ios .dialog-button:last-child:after {
  display: none !important;
}
.ios .dialog-button:first-child:last-child {
  border-radius: 0 0 var(--f7-dialog-border-radius) var(--f7-dialog-border-radius);
}
.ios .dialog-button.dialog-button-bold {
  font-weight: 500;
}
.ios .dialog-button[class*="color-"] {
  --f7-dialog-button-text-color: var(--f7-theme-color);
}
.ios .dialog-buttons-vertical .dialog-buttons {
  height: auto;
}
.ios .dialog-buttons-vertical .dialog-button {
  border-radius: 0;
}
.ios .dialog-buttons-vertical .dialog-button:after {
  content: '';
  position: absolute;
  background-color: var(--f7-dialog-border-divider-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.ios .dialog-buttons-vertical .dialog-button:last-child {
  border-radius: 0 0 var(--f7-dialog-border-radius) var(--f7-dialog-border-radius);
}
.ios .dialog-buttons-vertical .dialog-button:last-child:after {
  display: none !important;
}
.ios .dialog-no-buttons .dialog-inner {
  border-radius: var(--f7-dialog-border-radius);
}
.ios .dialog-no-buttons .dialog-inner:after {
  display: none !important;
}
.ios .dialog-input-field {
  margin-top: 15px;
}
.ios .dialog-input {
  padding: 0 5px;
}
.ios .dialog-input + .dialog-input {
  margin-top: 5px;
}
.ios .dialog-input-double + .dialog-input-double {
  margin-top: 0;
}
.ios .dialog-input-double + .dialog-input-double .dialog-input {
  border-top: 0;
  margin-top: 0;
}
.ios .dialog-preloader .dialog-title ~ .preloader,
.ios .dialog-preloader .dialog-text ~ .preloader {
  margin-top: 15px;
}
.ios .dialog-progress .dialog-title ~ .progressbar,
.ios .dialog-progress .dialog-text ~ .progressbar,
.ios .dialog-progress .dialog-title ~ .progressbar-infinite,
.ios .dialog-progress .dialog-text ~ .progressbar-infinite {
  margin-top: 15px;
}
.md .dialog.modal-out {
  transform: translate3d(0, -50%, 0) scale(0.815);
}
.md .dialog-title + .dialog-text {
  margin-top: 20px;
}
.md .dialog-text {
  line-height: 1.5;
}
.md .dialog-buttons {
  height: 48px;
  padding: 6px 8px;
  overflow: hidden;
  box-sizing: border-box;
  justify-content: flex-end;
}
.md .dialog-button {
  border-radius: 4px;
  min-width: 64px;
  padding: 0 8px;
  border: none;
  transition-duration: 300ms;
  transform: translate3d(0, 0, 0);
}
.md .dialog-button.dialog-button-bold {
  font-weight: 700;
}
.md .dialog-button + .dialog-button {
  margin-left: 4px;
}
.md .dialog-button[class*="color-"] {
  --f7-dialog-button-text-color: var(--f7-theme-color);
}
.md .dialog-buttons-vertical .dialog-buttons {
  padding: 0 0 8px 0;
}
.md .dialog-buttons-vertical .dialog-button {
  margin-left: 0;
  text-align: right;
  height: 48px;
  line-height: 48px;
  border-radius: 0;
  padding-left: 16px;
  padding-right: 16px;
}
.md .dialog-input {
  padding: 0;
  transition-duration: 200ms;
  position: relative;
}
.md .dialog-input + .dialog-input {
  margin-top: 16px;
}
.md .dialog-preloader .dialog-title,
.md .dialog-progress .dialog-title,
.md .dialog-preloader .dialog-inner,
.md .dialog-progress .dialog-inner {
  text-align: center;
}
.md .dialog-preloader .dialog-title ~ .preloader,
.md .dialog-preloader .dialog-text ~ .preloader {
  margin-top: 20px;
}
.md .dialog-progress .dialog-title ~ .progressbar,
.md .dialog-progress .dialog-text ~ .progressbar,
.md .dialog-progress .dialog-title ~ .progressbar-infinite,
.md .dialog-progress .dialog-text ~ .progressbar-infinite {
  margin-top: 16px;
}
.aurora .dialog.modal-out {
  transform: translate3d(0, -50%, 0) scale(0.815);
}
.aurora .dialog-title + .dialog-text {
  margin-top: 10px;
}
.aurora .dialog-text {
  line-height: 1.5;
}
.aurora .dialog-buttons {
  padding: var(--f7-dialog-inner-padding);
  padding-top: 0;
  overflow: hidden;
  box-sizing: border-box;
  justify-content: flex-end;
}
.aurora .dialog-button {
  border-radius: 4px;
  min-width: 64px;
  padding: 0 10px;
  border: none;
  transition-duration: 300ms;
  transform: translate3d(0, 0, 0);
  background: var(--f7-theme-color);
}
.aurora .dialog-button.dialog-button-bold {
  font-weight: 600;
}
.aurora .dialog-button + .dialog-button {
  margin-left: 16px;
}
.aurora .dialog-buttons-vertical .dialog-buttons {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}
.aurora .dialog-buttons-vertical .dialog-button {
  margin-left: 0;
  flex-shrink: 0;
}
.aurora .dialog-buttons-vertical .dialog-button + .dialog-button {
  margin-top: 5px;
}
.aurora .dialog-input-field {
  margin-top: 10px;
}
.aurora .dialog-input-field input.dialog-input {
  margin-top: 0;
}
.aurora .dialog-input {
  padding: 0 4px;
  transition-duration: 200ms;
  position: relative;
}
.aurora .dialog-input + .dialog-input {
  margin-top: 10px;
}
.aurora .dialog-input-double + .dialog-input-double {
  margin-top: 0;
}
.aurora .dialog-input-double + .dialog-input-double .dialog-input {
  border-top: 0;
  margin-top: 0;
}
.aurora .dialog-preloader .dialog-title,
.aurora .dialog-progress .dialog-title,
.aurora .dialog-preloader .dialog-inner,
.aurora .dialog-progress .dialog-inner {
  text-align: center;
}
.aurora .dialog-preloader .dialog-title ~ .preloader,
.aurora .dialog-preloader .dialog-text ~ .preloader {
  margin-top: 10px;
}
.aurora .dialog-progress .dialog-title ~ .progressbar,
.aurora .dialog-progress .dialog-text ~ .progressbar,
.aurora .dialog-progress .dialog-title ~ .progressbar-infinite,
.aurora .dialog-progress .dialog-text ~ .progressbar-infinite {
  margin-top: 15px;
}
/* === Popup === */
:root {
  --f7-popup-border-radius: 0px;
  --f7-popup-tablet-width: 630px;
  --f7-popup-tablet-height: 630px;
  --f7-popup-transition-duration: 400ms;
  --f7-popup-push-border-radius: 10px;
  --f7-popup-push-offset: var(--f7-safe-area-top);
  /*
  --f7-popup-tablet-border-radius: var(--f7-popup-border-radius);
  */
}
.ios {
  --f7-popup-box-shadow: none;
}
.md {
  --f7-popup-box-shadow: 0px 20px 44px rgba(0, 0, 0, 0.5);
}
.aurora {
  --f7-popup-tablet-border-radius: 4px;
  --f7-popup-box-shadow: 0px 20px 44px rgba(0, 0, 0, 0.5);
}
.popup-backdrop {
  z-index: 10500;
}
.popup {
  position: absolute;
  left: 0;
  top: 0px;
  width: 100%;
  height: 100%;
  display: none;
  box-sizing: border-box;
  transition-property: transform;
  transform: translate3d(0, 100%, 0);
  background: #fff;
  z-index: 11000;
  overflow: hidden;
  border-radius: var(--f7-popup-border-radius);
}
.popup.modal-in,
.popup.modal-out {
  transition-duration: var(--f7-popup-transition-duration);
}
.popup.not-animated {
  transition-duration: 0ms;
}
.popup.modal-in {
  display: block;
  transform: translate3d(0, 0, 0);
}
.popup.modal-out {
  transform: translate3d(0, 100%, 0);
}
.popup.swipe-close-to-top.modal-out {
  transform: translate3d(0, -100%, 0);
}
@media (min-width: 630px) and (min-height: 630px) {
  .popup:not(.popup-tablet-fullscreen) {
    --f7-safe-area-top: 0px;
    width: var(--f7-popup-tablet-width);
    height: var(--f7-popup-tablet-height);
    left: 50%;
    top: 50%;
    margin-left: calc(-1 * var(--f7-popup-tablet-width) / 2);
    margin-top: calc(-1 * var(--f7-popup-tablet-height) / 2);
    transform: translate3d(0, 100vh, 0);
    box-shadow: var(--f7-popup-box-shadow);
    border-radius: var(--f7-popup-tablet-border-radius, var(--f7-popup-border-radius));
  }
  .popup:not(.popup-tablet-fullscreen).modal-in {
    transform: translate3d(0, 0, 0);
  }
  .popup:not(.popup-tablet-fullscreen).modal-out {
    transform: translate3d(0, 100vh, 0);
  }
  .popup:not(.popup-tablet-fullscreen).swipe-close-to-top.modal-out {
    transform: translate3d(0, -100vh, 0);
  }
}
html.with-modal-popup .framework7-root > .views .page-content,
html.with-modal-popup .framework7-root > .view .page-content,
html.with-modal-popup .framework7-root > .panel .page-content {
  overflow: hidden;
  -webkit-overflow-scrolling: auto;
}
html.with-modal-popup-push .popup-push,
html.with-modal-popup-push-closing .popup-push {
  top: calc(var(--f7-popup-push-offset) + 10px);
  height: calc(100% - var(--f7-popup-push-offset) - 10px);
  border-radius: var(--f7-popup-push-border-radius) var(--f7-popup-push-border-radius) 0 0;
}
html.with-modal-popup-push .popup-push .view,
html.with-modal-popup-push-closing .popup-push .view,
html.with-modal-popup-push .popup-push .page,
html.with-modal-popup-push-closing .popup-push .page {
  --f7-safe-area-top: 0px;
}
html.with-modal-popup-push .framework7-root,
html.with-modal-popup-push-closing .framework7-root {
  background: #000;
}
html.with-modal-popup-push .framework7-root > .views,
html.with-modal-popup-push-closing .framework7-root > .views,
html.with-modal-popup-push .framework7-root > .view,
html.with-modal-popup-push-closing .framework7-root > .view {
  transition-duration: var(--f7-popup-transition-duration);
}
html.with-modal-popup-push .framework7-root > .views,
html.with-modal-popup-push .framework7-root > .view {
  border-radius: var(--f7-popup-push-border-radius) var(--f7-popup-push-border-radius) 0 0;
  transform: translate3d(0, 0, 0px) scale(var(--f7-popup-push-scale, 1));
}
/* === Login Screen === */
:root {
  --f7-login-screen-blocks-max-width: 480px;
  /*
   --f7-login-screen-list-button-text-color: var(--f7-theme-color);
   */
  --f7-login-screen-title-text-align: center;
  --f7-login-screen-title-text-color: inherit;
  --f7-login-screen-title-letter-spacing: 0;
  --f7-login-screen-title-font-weight: 600;
  --f7-login-screen-title-font-size: 28px;
  --f7-login-screen-content-bg-color: #fff;
  --f7-login-screen-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-login-screen-bg-color: #121212;
  --f7-login-screen-content-bg-color: transparent;
}
.ios {
  --f7-login-screen-blocks-margin-vertical: 25px;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-login-screen-bg-color: #000;
}
.md {
  --f7-login-screen-blocks-margin-vertical: 24px;
}
.aurora {
  --f7-login-screen-blocks-margin-vertical: 15px;
}
.login-screen {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  display: none;
  box-sizing: border-box;
  transition-property: transform;
  transform: translate3d(0, 100%, 0);
  background: var(--f7-login-screen-bg-color);
  z-index: 11000;
}
.login-screen.modal-in,
.login-screen.modal-out {
  transition-duration: 400ms;
}
.login-screen.not-animated {
  transition-duration: 0ms;
}
.login-screen.modal-in {
  display: block;
  transform: translate3d(0, 0, 0);
}
.login-screen.modal-out {
  transform: translate3d(0, 100%, 0);
}
.login-screen-content,
.login-screen-page,
.login-screen .page {
  background: var(--f7-login-screen-content-bg-color);
}
.login-screen-content .list-button,
.login-screen-page .list-button {
  text-align: center;
  color: var(--f7-login-screen-list-button-text-color, var(--f7-theme-color));
}
.login-screen-content .login-screen-title,
.login-screen-page .login-screen-title,
.login-screen-content .list,
.login-screen-page .list,
.login-screen-content .block,
.login-screen-page .block {
  margin: var(--f7-login-screen-blocks-margin-vertical) auto;
}
.login-screen-content .login-screen-title,
.login-screen-page .login-screen-title,
.login-screen-content .list,
.login-screen-page .list,
.login-screen-content .block,
.login-screen-page .block,
.login-screen-content .block-footer,
.login-screen-page .block-footer,
.login-screen-content .block-header,
.login-screen-page .block-header {
  max-width: var(--f7-login-screen-blocks-max-width);
}
.login-screen-content .list ul,
.login-screen-page .list ul {
  background: none;
}
.login-screen-content .list ul:before,
.login-screen-page .list ul:before,
.login-screen-content .list ul:after,
.login-screen-page .list ul:after {
  display: none !important;
}
.login-screen-content .block-footer,
.login-screen-page .block-footer,
.login-screen-content .block-header,
.login-screen-page .block-header {
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}
.login-screen-title {
  text-align: var(--f7-login-screen-title-text-align);
  font-size: var(--f7-login-screen-title-font-size);
  font-weight: var(--f7-login-screen-title-font-weight);
  color: var(--f7-login-screen-title-text-color);
  letter-spacing: var(--f7-login-screen-title-letter-spacing);
}
.login-screen-page,
.login-screen > .view > .page,
.login-screen > .page {
  display: flex;
  flex-direction: column;
}
.login-screen-page .page-content,
.login-screen > .view > .page .page-content,
.login-screen > .page .page-content,
.login-screen-page .login-screen-content,
.login-screen > .view > .page .login-screen-content,
.login-screen > .page .login-screen-content {
  margin-top: auto;
  margin-bottom: auto;
  height: auto;
  max-height: 100%;
  width: 100%;
}
.theme-dark .login-screen-content .list ul,
.theme-dark .login-screen-content .block-strong,
.theme-dark .login-screen-page .list ul,
.theme-dark .login-screen-page .block-strong,
.theme-dark.login-screen-page .list ul,
.theme-dark.login-screen-page .block-strong {
  background-color: transparent;
}
/* === Popover === */
:root {
  --f7-popover-width: 260px;
}
.ios {
  --f7-popover-border-radius: 13px;
  --f7-popover-box-shadow: none;
  --f7-popover-actions-icon-size: 28px;
  --f7-popover-bg-color: rgba(255, 255, 255, 0.95);
  --f7-popover-actions-label-text-color: rgba(0, 0, 0, 0.45);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-popover-bg-color: rgba(30, 30, 30, 0.95);
  --f7-popover-actions-label-text-color: rgba(255, 255, 255, 0.55);
}
.md {
  --f7-popover-border-radius: 4px;
  --f7-popover-box-shadow: var(--f7-elevation-8);
  --f7-popover-actions-icon-size: 24px;
  --f7-popover-bg-color: #fff;
  --f7-popover-actions-label-text-color: rgba(0, 0, 0, 0.54);
}
.md .theme-dark,
.md.theme-dark {
  --f7-popover-bg-color: #1c1c1d;
  --f7-popover-actions-label-text-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-popover-width: 200px;
  --f7-popover-border-radius: 4px;
  --f7-popover-box-shadow: 0 0 3px 0 rgba(0, 0, 0, 0.1), 0 5px 11px 0 rgba(0,0,0,0.28);
  --f7-popover-actions-icon-size: 24px;
  --f7-popover-bg-color: #fff;
  --f7-popover-actions-label-text-color: rgba(0, 0, 0, 0.6);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-popover-bg-color: #1c1c1d;
  --f7-popover-actions-label-text-color: rgba(255, 255, 255, 0.6);
}
.popover {
  width: var(--f7-popover-width);
  z-index: 13500;
  margin: 0;
  top: 0;
  opacity: 0;
  left: 0;
  position: absolute;
  display: none;
  transition-duration: 300ms;
  background-color: var(--f7-popover-bg-color);
  border-radius: var(--f7-popover-border-radius);
  box-shadow: var(--f7-popover-box-shadow);
}
.popover .list {
  margin: 0;
}
.popover .list ul {
  background: none;
}
.popover .list:first-child ul:before {
  display: none !important;
}
.popover .list:last-child ul:after {
  display: none !important;
}
.popover .list:first-child ul {
  border-radius: var(--f7-popover-border-radius) var(--f7-popover-border-radius) 0 0;
}
.popover .list:first-child li:first-child,
.popover .list:first-child li:first-child a,
.popover .list:first-child li:first-child > label {
  border-radius: var(--f7-popover-border-radius) var(--f7-popover-border-radius) 0 0;
}
.popover .list:last-child ul {
  border-radius: 0 0 var(--f7-popover-border-radius) var(--f7-popover-border-radius);
}
.popover .list:last-child li:last-child,
.popover .list:last-child li:last-child a,
.popover .list:last-child li:last-child > label {
  border-radius: 0 0 var(--f7-popover-border-radius) var(--f7-popover-border-radius);
}
.popover .list:first-child:last-child li:first-child:last-child,
.popover .list:first-child:last-child li:first-child:last-child a,
.popover .list:first-child:last-child li:first-child:last-child > label,
.popover .list:first-child:last-child ul {
  border-radius: var(--f7-popover-border-radius);
}
.popover .list + .list {
  margin-top: var(--f7-list-margin-vertical);
}
.popover.modal-in {
  opacity: 1;
}
.popover.not-animated {
  transition-duration: 0ms;
}
.popover-inner {
  overflow: auto;
  -webkit-overflow-scrolling: touch;
}
.popover-from-actions .item-link i.icon {
  width: var(--f7-popover-actions-icon-size);
  height: var(--f7-popover-actions-icon-size);
  font-size: var(--f7-popover-actions-icon-size);
}
.popover-from-actions-bold {
  font-weight: 600;
}
.popover-from-actions-label {
  line-height: 1.3;
  position: relative;
  display: flex;
  align-items: center;
  padding: var(--f7-actions-label-padding);
  color: var(--f7-popover-actions-label-text-color);
  font-size: var(--f7-actions-label-font-size);
  justify-content: var(--f7-actions-label-justify-content);
}
.popover-from-actions-label:after {
  content: '';
  position: absolute;
  background-color: var(--f7-list-item-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.popover-from-actions-label:last-child:after {
  display: none !important;
}
.ios .popover {
  transform: none;
  transition-property: opacity;
}
.ios .popover-angle {
  width: 26px;
  height: 26px;
  position: absolute;
  left: -26px;
  top: 0;
  z-index: 100;
  overflow: hidden;
}
.ios .popover-angle:after {
  content: '';
  background: var(--f7-popover-bg-color);
  width: 26px;
  height: 26px;
  position: absolute;
  left: 0;
  top: 0;
  border-radius: 3px;
  transform: rotate(45deg);
}
.ios .popover-angle.on-left {
  left: -26px;
}
.ios .popover-angle.on-left:after {
  left: 19px;
  top: 0;
}
.ios .popover-angle.on-right {
  left: 100%;
}
.ios .popover-angle.on-right:after {
  left: -19px;
  top: 0;
}
.ios .popover-angle.on-top {
  left: 0;
  top: -26px;
}
.ios .popover-angle.on-top:after {
  left: 0;
  top: 19px;
}
.ios .popover-angle.on-bottom {
  left: 0;
  top: 100%;
}
.ios .popover-angle.on-bottom:after {
  left: 0;
  top: -19px;
}
.md .popover {
  transform: scale(0.85, 0.6);
  transition-property: opacity, transform;
}
.md .popover.modal-in {
  opacity: 1;
  transform: scale(1);
}
.md .popover.modal-out {
  opacity: 0;
  transform: scale(1);
}
.md .popover-on-top {
  transform-origin: center bottom;
}
.md .popover-on-top.popover-on-right {
  transform-origin: left bottom;
}
.md .popover-on-top.popover-on-left {
  transform-origin: right bottom;
}
.md .popover-on-middle {
  transform-origin: center center;
}
.md .popover-on-middle.popover-on-right {
  transform-origin: left center;
}
.md .popover-on-middle.popover-on-left {
  transform-origin: right center;
}
.md .popover-on-bottom {
  transform-origin: center top;
}
.md .popover-on-bottom.popover-on-right {
  transform-origin: left top;
}
.md .popover-on-bottom.popover-on-left {
  transform-origin: right top;
}
.aurora .popover {
  transform: none;
  transition-property: opacity;
}
.aurora .popover-angle {
  width: 18px;
  height: 18px;
  position: absolute;
  left: -18px;
  top: 0;
  z-index: 100;
  overflow: hidden;
}
.aurora .popover-angle:after {
  content: '';
  background: var(--f7-popover-bg-color);
  width: 18px;
  height: 18px;
  position: absolute;
  left: 0;
  top: 0;
  border-radius: 2px;
  transform: rotate(45deg);
}
.aurora .popover-angle.on-left {
  left: -18px;
}
.aurora .popover-angle.on-left:after {
  left: 13px;
  top: 0;
}
.aurora .popover-angle.on-right {
  left: 100%;
}
.aurora .popover-angle.on-right:after {
  left: -13px;
  top: 0;
}
.aurora .popover-angle.on-top {
  left: 0;
  top: -18px;
}
.aurora .popover-angle.on-top:after {
  left: 0;
  top: 13px;
}
.aurora .popover-angle.on-bottom {
  left: 0;
  top: 100%;
}
.aurora .popover-angle.on-bottom:after {
  left: 0;
  top: -13px;
}
/* === Actions === */
:root {
  --f7-actions-grid-button-font-size: 12px;
  --f7-actions-grid-button-text-color: #757575;
}
:root .theme-dark,
:root.theme-dark {
  --f7-actions-label-text-color: rgba(255, 255, 255, 0.55);
}
.ios {
  --f7-actions-border-radius: 13px;
  /*
  --f7-actions-button-text-color: var(--f7-theme-color);
  */
  --f7-actions-button-padding: 0px;
  --f7-actions-button-text-align: center;
  --f7-actions-button-height: 57px;
  --f7-actions-button-height-landscape: 44px;
  --f7-actions-button-font-size: 20px;
  --f7-actions-button-icon-size: 28px;
  --f7-actions-button-justify-content: center;
  --f7-actions-label-padding: 8px 10px;
  --f7-actions-label-font-size: 13px;
  --f7-actions-label-justify-content: center;
  --f7-actions-group-border-color: transparent;
  --f7-actions-group-margin: 8px;
  --f7-actions-grid-button-icon-size: 48px;
  --f7-actions-bg-color: rgba(255, 255, 255, 0.95);
  --f7-actions-bg-color-rgb: 255, 255, 255;
  --f7-actions-button-border-color: rgba(0, 0, 0, 0.2);
  --f7-actions-button-pressed-bg-color: rgba(230, 230, 230, 0.9);
  --f7-actions-button-pressed-bg-color-rgb: 230, 230, 230;
  --f7-actions-label-text-color: #8a8a8a;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-actions-bg-color: rgba(45, 45, 45, 0.95);
  --f7-actions-bg-color-rgb: 45, 45, 45;
  --f7-actions-button-border-color: rgba(255, 255, 255, 0.15);
  --f7-actions-button-pressed-bg-color: rgba(50, 50, 50, 0.9);
  --f7-actions-button-pressed-bg-color-rgb: 50, 50, 50;
}
.md {
  --f7-actions-border-radius: 0px;
  --f7-actions-button-border-color: transparent;
  --f7-actions-button-padding: 0 16px;
  --f7-actions-button-text-align: left;
  --f7-actions-button-height: 48px;
  --f7-actions-button-height-landscape: 48px;
  --f7-actions-button-font-size: 16px;
  --f7-actions-button-icon-size: 24px;
  --f7-actions-button-justify-content: space-between;
  --f7-actions-label-padding: 12px 16px;
  --f7-actions-label-font-size: 16px;
  --f7-actions-label-justify-content: flex-start;
  --f7-actions-group-margin: 0px;
  --f7-actions-grid-button-icon-size: 48px;
  --f7-actions-bg-color: #fff;
  --f7-actions-button-text-color: rgba(0, 0, 0, 0.87);
  --f7-actions-button-pressed-bg-color: #e5e5e5;
  --f7-actions-label-text-color: rgba(0, 0, 0, 0.54);
  --f7-actions-group-border-color: rgba(0, 0, 0, 0.12);
}
.md .theme-dark,
.md.theme-dark {
  --f7-actions-bg-color: #202020;
  --f7-actions-button-text-color: #fff;
  --f7-actions-button-pressed-bg-color: #2e2e2e;
  --f7-actions-group-border-color: rgba(255, 255, 255, 0.15);
}
.aurora {
  --f7-actions-border-radius: 4px;
  --f7-actions-button-padding: 0 16px;
  --f7-actions-button-text-align: center;
  --f7-actions-button-height: 32px;
  --f7-actions-button-height-landscape: 32px;
  --f7-actions-button-font-size: 14px;
  --f7-actions-button-icon-size: 18px;
  --f7-actions-button-justify-content: space-between;
  --f7-actions-label-padding: 10px 16px;
  --f7-actions-label-font-size: 12px;
  --f7-actions-label-justify-content: center;
  --f7-actions-group-margin: 16px;
  --f7-actions-grid-button-icon-size: 32px;
  --f7-actions-bg-color: #fff;
  --f7-actions-button-border-color: rgba(0, 0, 0, 0.12);
  /*
    --f7-actions-button-text-color: var(--f7-theme-color);
    */
  --f7-actions-button-pressed-bg-color: #e5e5e5;
  --f7-actions-label-text-color: rgba(0, 0, 0, 0.5);
  --f7-actions-group-border-color: rgba(0, 0, 0, 0.1);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-actions-bg-color: #202020;
  --f7-actions-button-text-color: #fff;
  --f7-actions-button-border-color: rgba(255, 255, 255, 0.15);
  --f7-actions-button-pressed-bg-color: #2e2e2e;
  --f7-actions-group-border-color: rgba(255, 255, 255, 0.15);
}
.actions-modal {
  position: absolute;
  left: 0;
  bottom: 0;
  z-index: 13500;
  width: 100%;
  transform: translate3d(0, 100%, 0);
  display: none;
  max-height: 100%;
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  transition-property: transform;
}
.actions-modal.modal-in,
.actions-modal.modal-out {
  transition-duration: 300ms;
}
.actions-modal.not-animated {
  transition-duration: 0ms;
}
.actions-modal.modal-in {
  transform: translate3d(0, calc(-1 * var(--f7-safe-area-bottom)), 0);
}
.actions-modal.modal-out {
  z-index: 13499;
  transform: translate3d(0, 100%, 0);
}
@media (min-width: 496px) {
  .actions-modal {
    width: 480px;
    left: 50%;
    margin-left: -240px;
  }
}
@media (orientation: landscape) {
  .actions-modal {
    --f7-actions-button-height: var(--f7-actions-button-height-landscape);
  }
}
.actions-group {
  overflow: hidden;
  position: relative;
  margin: var(--f7-actions-group-margin);
  border-radius: var(--f7-actions-border-radius);
  transform: translate3d(0, 0, 0);
}
.actions-group:after {
  content: '';
  position: absolute;
  background-color: var(--f7-actions-group-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.actions-group:last-child:after {
  display: none !important;
}
.actions-button,
.actions-label {
  width: 100%;
  font-weight: normal;
  margin: 0;
  box-sizing: border-box;
  display: block;
  position: relative;
  overflow: hidden;
  text-align: var(--f7-actions-button-text-align);
  background: var(--f7-actions-bg-color);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-modals .actions-button,
  .ios-translucent-modals .actions-label {
    background-color: rgba(var(--f7-actions-bg-color-rgb), 0.8);
    -webkit-backdrop-filter: saturate(180%) blur(20px);
            backdrop-filter: saturate(180%) blur(20px);
  }
}
.actions-button:after,
.actions-label:after {
  content: '';
  position: absolute;
  background-color: var(--f7-actions-button-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.actions-button:first-child,
.actions-label:first-child {
  border-radius: var(--f7-actions-border-radius) var(--f7-actions-border-radius) 0 0;
}
.actions-button:last-child,
.actions-label:last-child {
  border-radius: 0 0 var(--f7-actions-border-radius) var(--f7-actions-border-radius);
}
.actions-button:last-child:after,
.actions-label:last-child:after {
  display: none !important;
}
.actions-button:first-child:last-child,
.actions-label:first-child:last-child {
  border-radius: var(--f7-actions-border-radius);
}
.actions-button a,
.actions-label a {
  text-decoration: none;
  color: inherit;
  display: block;
}
.actions-button b,
.actions-label b,
.actions-button.actions-button-bold,
.actions-label.actions-button-bold {
  font-weight: 600;
}
.actions-button {
  cursor: pointer;
  display: flex;
  color: var(--f7-actions-button-text-color, var(--f7-theme-color));
  font-size: var(--f7-actions-button-font-size);
  height: var(--f7-actions-button-height);
  line-height: var(--f7-actions-button-height);
  padding: var(--f7-actions-button-padding);
  justify-content: var(--f7-actions-button-justify-content);
  z-index: 10;
}
.actions-button.active-state {
  background-color: var(--f7-actions-button-pressed-bg-color) !important;
}
.actions-button[class*="color-"] {
  color: var(--f7-theme-color);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-modals .actions-button.active-state {
    background-color: rgba(var(--f7-actions-button-pressed-bg-color-rgb), 0.8);
    -webkit-backdrop-filter: saturate(180%) blur(20px);
            backdrop-filter: saturate(180%) blur(20px);
  }
}
.actions-button-media {
  flex-shrink: 0;
  display: flex;
  align-items: center;
}
.actions-button-media i.icon {
  width: var(--f7-actions-button-icon-size);
  height: var(--f7-actions-button-icon-size);
  font-size: var(--f7-actions-button-icon-size);
}
.actions-button a,
.actions-button-text {
  position: relative;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
.actions-button-text {
  width: 100%;
  flex-shrink: 1;
  text-align: var(--f7-actions-button-text-align);
}
.actions-label {
  line-height: 1.3;
  display: flex;
  align-items: center;
  font-size: var(--f7-actions-label-font-size);
  color: var(--f7-actions-label-text-color);
  padding: var(--f7-actions-label-padding);
  justify-content: var(--f7-actions-label-justify-content);
  min-height: var(--f7-actions-label-min-height, var(--f7-actions-button-height));
}
.actions-label[class*=" color-"] {
  --f7-actions-label-text-color: var(--f7-theme-color);
}
.actions-grid .actions-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
  border-radius: 0;
  background: var(--f7-actions-bg-color);
  margin-top: 0;
}
.actions-grid .actions-group:first-child {
  border-radius: var(--f7-actions-border-radius) var(--f7-actions-border-radius) 0 0;
}
.actions-grid .actions-group:last-child {
  border-radius: 0 0 var(--f7-actions-border-radius) var(--f7-actions-border-radius);
}
.actions-grid .actions-group:first-child:last-child {
  border-radius: var(--f7-actions-border-radius);
}
.actions-grid .actions-group:not(:last-child) {
  margin-bottom: 0;
}
.actions-grid .actions-button,
.actions-grid .actions-label {
  border-radius: 0 !important;
  background: none;
}
.actions-grid .actions-button {
  width: 33.33333333%;
  display: block;
  color: var(--f7-actions-grid-button-text-color);
  height: auto;
  line-height: 1;
  padding: 16px;
}
.actions-grid .actions-button:after {
  display: none !important;
}
.actions-grid .actions-button-media {
  margin-left: auto !important;
  margin-right: auto !important;
  width: var(--f7-actions-grid-button-icon-size);
  height: var(--f7-actions-grid-button-icon-size);
}
.actions-grid .actions-button-media i.icon {
  width: var(--f7-actions-grid-button-icon-size);
  height: var(--f7-actions-grid-button-icon-size);
  font-size: var(--f7-actions-grid-button-icon-size);
}
.actions-grid .actions-button-text {
  margin-left: 0 !important;
  text-align: center !important;
  margin-top: 8px;
  line-height: 1.33em;
  height: 1.33em;
  font-size: var(--f7-actions-grid-button-font-size);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-modals .actions-grid .actions-group {
    background-color: rgba(var(--f7-actions-bg-color-rgb), 0.8);
    -webkit-backdrop-filter: saturate(180%) blur(20px);
            backdrop-filter: saturate(180%) blur(20px);
  }
}
.ios .actions-button-media {
  margin-left: 16px;
}
.ios .actions-button-media + .actions-button-text {
  text-align: left;
  margin-left: 16px;
}
.md .actions-button {
  transition-duration: 300ms;
}
.md .actions-button-media {
  min-width: 40px;
}
.md .actions-button-media + .actions-button-text {
  margin-left: 16px;
}
.aurora .actions-button-media {
  margin-left: 16px;
}
.aurora .actions-button-media + .actions-button-text {
  text-align: left;
  margin-left: 16px;
}
/* === Sheet Modal === */
:root {
  --f7-sheet-height: 260px;
  --f7-sheet-border-color: transparent;
  --f7-sheet-transition-duration: 300ms;
  --f7-sheet-push-border-radius: 10px;
  --f7-sheet-push-offset: var(--f7-safe-area-top);
  --f7-sheet-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-sheet-bg-color: #202020;
}
.ios {
  --f7-sheet-border-color: var(--f7-bars-border-color);
}
.sheet-backdrop {
  z-index: 11000;
}
.sheet-modal {
  position: absolute;
  left: 0;
  bottom: 0;
  width: 100%;
  height: var(--f7-sheet-height);
  display: none;
  box-sizing: border-box;
  transition-property: transform;
  transform: translate3d(0, 100%, 0);
  background: var(--f7-sheet-bg-color);
  z-index: 12500;
}
.sheet-modal.modal-in,
.sheet-modal.modal-out {
  transition-duration: var(--f7-sheet-transition-duration);
}
.sheet-modal.not-animated {
  transition-duration: 0ms;
}
.sheet-modal.modal-in {
  display: block;
  transform: translate3d(0, 0, 0);
}
.sheet-modal.modal-in-swipe-step {
  display: block;
  transform: translate3d(0, var(--f7-sheet-swipe-step, 0), 0);
}
.sheet-modal.modal-out {
  transform: translate3d(0, 100%, 0);
}
.sheet-modal .sheet-modal-inner {
  height: 100%;
  position: relative;
  overflow: hidden;
}
.sheet-modal .toolbar {
  --f7-safe-area-bottom: 0px;
  position: relative;
  width: 100%;
}
.sheet-modal .toolbar:after,
.sheet-modal .toolbar:before {
  display: none;
}
.sheet-modal .toolbar + .sheet-modal-inner {
  height: calc(100% - var(--f7-toolbar-height));
}
.sheet-modal .toolbar + .sheet-modal-inner .page-content {
  --f7-page-toolbar-top-offset: 0px;
  --f7-page-toolbar-bottom-offset: 0px;
}
.sheet-modal-top:after {
  content: '';
  position: absolute;
  background-color: var(--f7-sheet-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.sheet-modal-top:after {
  z-index: 600;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  transform-style: preserve-3d;
}
.sheet-modal-bottom,
.sheet-modal:not(.sheet-modal-top) {
  --f7-safe-area-top: 0px;
}
.sheet-modal-bottom:before,
.sheet-modal:not(.sheet-modal-top):before {
  content: '';
  position: absolute;
  background-color: var(--f7-sheet-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.sheet-modal-bottom:before,
.sheet-modal:not(.sheet-modal-top):before {
  z-index: 600;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  transform-style: preserve-3d;
}
.sheet-modal-top {
  --f7-safe-area-bottom: 0px;
  bottom: auto;
  top: 0;
  transform: translate3d(0, -100%, 0);
}
.sheet-modal-top.modal-out {
  transform: translate3d(0, -100%, 0);
}
.sheet-modal-top .toolbar-bottom {
  position: absolute;
}
.sheet-modal-top .page-content {
  padding-top: var(--f7-safe-area-top);
}
html.with-modal-sheet-push .sheet-modal-push,
html.with-modal-sheet-push-closing .sheet-modal-push {
  border-radius: var(--f7-sheet-push-border-radius) var(--f7-sheet-push-border-radius) 0 0;
  overflow: hidden;
}
html.with-modal-sheet-push .sheet-modal-push .view,
html.with-modal-sheet-push-closing .sheet-modal-push .view,
html.with-modal-sheet-push .sheet-modal-push .page,
html.with-modal-sheet-push-closing .sheet-modal-push .page {
  --f7-safe-area-top: 0px;
}
html.with-modal-sheet-push .sheet-modal-push.sheet-modal-top,
html.with-modal-sheet-push-closing .sheet-modal-push.sheet-modal-top {
  border-radius: 0 0 var(--f7-sheet-push-border-radius) var(--f7-sheet-push-border-radius);
}
html.with-modal-sheet-push .framework7-root,
html.with-modal-sheet-push-closing .framework7-root {
  background: #000;
}
html.with-modal-sheet-push .framework7-root > .views,
html.with-modal-sheet-push-closing .framework7-root > .views,
html.with-modal-sheet-push .framework7-root > .view,
html.with-modal-sheet-push-closing .framework7-root > .view {
  transition-duration: var(--f7-sheet-transition-duration);
}
html.with-modal-sheet-push .framework7-root > .views,
html.with-modal-sheet-push .framework7-root > .view {
  border-radius: var(--f7-sheet-push-border-radius);
  transform: translate3d(0, 0, 0px) scale(var(--f7-sheet-push-scale, 1));
}
.md .sheet-modal .toolbar a.link:not(.tab-link) {
  flex-shrink: 0;
}
/* === Toast === */
:root {
  --f7-toast-text-color: #fff;
  --f7-toast-font-size: 14px;
  --f7-toast-icon-size: 48px;
}
.ios {
  --f7-toast-bg-color: rgba(0, 0, 0, 0.75);
  --f7-toast-bg-color-rgb: 0, 0, 0;
  --f7-toast-padding-horizontal: 16px;
  --f7-toast-padding-vertical: 12px;
  --f7-toast-border-radius: 8px;
  --f7-toast-button-min-width: 64px;
}
.md {
  --f7-toast-bg-color: #323232;
  --f7-toast-padding-horizontal: 24px;
  --f7-toast-padding-vertical: 14px;
  --f7-toast-border-radius: 4px;
  --f7-toast-button-min-width: 64px;
}
.aurora {
  --f7-toast-bg-color: rgba(0, 0, 0, 0.85);
  --f7-toast-padding-horizontal: 10px;
  --f7-toast-padding-vertical: 10px;
  --f7-toast-border-radius: 4px;
  --f7-toast-button-min-width: 32px;
}
.toast {
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
  transition-property: transform, opacity;
  position: absolute;
  max-width: 568px;
  z-index: 20000;
  color: var(--f7-toast-text-color);
  font-size: var(--f7-toast-font-size);
  box-sizing: border-box;
  background-color: var(--f7-toast-bg-color);
  opacity: 0;
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-modals .toast {
    background-color: rgba(var(--f7-toast-bg-color-rgb), 0.8);
    -webkit-backdrop-filter: saturate(180%) blur(20px);
            backdrop-filter: saturate(180%) blur(20px);
  }
}
.toast.modal-in {
  opacity: 1;
}
.toast .toast-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
  padding: var(--f7-toast-padding-vertical) var(--f7-toast-padding-horizontal);
}
.toast .toast-text {
  line-height: 20px;
  flex-shrink: 1;
  min-width: 0;
}
.toast .toast-button {
  flex-shrink: 0;
  min-width: var(--f7-toast-button-min-width);
  margin-top: -8px;
  margin-bottom: -8px;
}
.toast.toast-with-icon .toast-content {
  display: block;
  text-align: center;
}
.toast.toast-with-icon .toast-text {
  text-align: center;
}
.toast.toast-with-icon .toast-icon .f7-icons,
.toast.toast-with-icon .toast-icon .material-icons {
  font-size: var(--f7-toast-icon-size);
}
.toast.toast-center {
  top: 50%;
}
.toast.toast-top {
  margin-top: var(--f7-safe-area-top);
}
.ios .toast {
  transition-duration: 300ms;
  width: 100%;
  left: 0;
}
.ios .toast.toast-top {
  top: 0;
  transform: translate3d(0, -100%, 0);
}
.ios .toast.toast-top.modal-in {
  transform: translate3d(0, 0%, 0);
}
.ios .toast.toast-center {
  width: auto;
  left: 50%;
  border-radius: var(--f7-toast-border-radius);
  transform: translate3d(-50%, -50%, 0);
}
.ios .toast.toast-center.modal-in {
  transform: translate3d(-50%, -50%, 0);
}
.ios .toast.toast-bottom {
  bottom: 0;
  transform: translate3d(0, 100%, 0);
}
.ios .toast.toast-bottom.modal-in {
  transform: translate3d(0, 0%, 0);
}
@media (max-width: 568px) {
  .ios .toast.toast-top {
    margin-top: 0;
  }
  .ios .toast.toast-top .toast-content {
    padding-top: calc(var(--f7-toast-padding-vertical) + var(--f7-safe-area-top));
  }
  .ios .toast.toast-bottom .toast-content {
    padding-bottom: calc(var(--f7-toast-padding-vertical) + var(--f7-safe-area-bottom));
  }
}
@media (min-width: 569px) {
  .ios .toast {
    left: 50%;
    margin-left: -284px;
    border-radius: var(--f7-toast-border-radius);
  }
  .ios .toast.toast-top {
    top: 16px;
  }
  .ios .toast.toast-center {
    margin-left: 0;
  }
  .ios .toast.toast-bottom {
    margin-bottom: calc(16px + var(--f7-safe-area-bottom));
  }
}
@media (min-width: 1024px) {
  .ios .toast {
    margin-left: 0;
    width: auto;
  }
  .ios .toast.toast-bottom,
  .ios .toast.toast-top {
    left: 16px;
  }
}
.ios .toast-button {
  margin-left: 16px;
  margin-right: calc(-1 * var(--f7-button-padding-horizontal));
}
.md .toast {
  transition-duration: 200ms;
  border-radius: var(--f7-toast-border-radius);
  left: 8px;
  width: calc(100% - 16px);
  transform: scale(0.9);
}
.md .toast.modal-in {
  transform: scale(1);
}
.md .toast.modal-out {
  transform: scale(1);
}
.md .toast.toast-top {
  top: 8px;
}
.md .toast.toast-center {
  left: 50%;
  width: auto;
  transform: scale(0.9) translate3d(-55%, -55%, 0);
}
.md .toast.toast-center.modal-in {
  transform: scale(1) translate3d(-50%, -50%, 0);
}
.md .toast.toast-center.modal-out {
  transform: scale(1) translate3d(-50%, -50%, 0);
}
.md .toast.toast-bottom {
  bottom: calc(8px + var(--f7-safe-area-bottom));
}
@media (min-width: 584px) {
  .md .toast {
    left: 50%;
    margin-left: -284px;
  }
  .md .toast.toast-center {
    margin-left: 0;
  }
}
@media (min-width: 1024px) {
  .md .toast {
    margin-left: 0;
    width: auto;
  }
  .md .toast.toast-bottom,
  .md .toast.toast-top {
    left: 24px;
  }
  .md .toast.toast-bottom {
    bottom: calc(24px + var(--f7-safe-area-bottom));
  }
  .md .toast.toast-top {
    top: 24px;
  }
}
.md .toast-button {
  margin-left: 16px;
  margin-right: -8px;
}
.aurora .toast {
  transition-duration: 200ms;
  border-radius: var(--f7-toast-border-radius);
  left: 10px;
  width: calc(100% - 20px);
  transform: scale(0.9);
}
.aurora .toast.modal-in {
  transform: scale(1);
}
.aurora .toast.modal-out {
  transform: scale(1);
}
.aurora .toast.toast-top {
  top: 10px;
}
.aurora .toast.toast-center {
  left: 50%;
  width: auto;
  transform: scale(0.9) translate3d(-55%, -55%, 0);
}
.aurora .toast.toast-center.modal-in {
  transform: scale(1) translate3d(-50%, -50%, 0);
}
.aurora .toast.toast-center.modal-out {
  transform: scale(1) translate3d(-50%, -50%, 0);
}
.aurora .toast.toast-bottom {
  bottom: calc(10px + var(--f7-safe-area-bottom));
}
@media (min-width: 584px) {
  .aurora .toast {
    left: 50%;
    margin-left: -284px;
  }
  .aurora .toast.toast-center {
    margin-left: 0;
  }
}
@media (min-width: 1024px) {
  .aurora .toast {
    margin-left: 0;
    width: auto;
  }
  .aurora .toast.toast-bottom,
  .aurora .toast.toast-top {
    left: 10px;
  }
}
.aurora .toast-button {
  margin-left: 10px;
}
/* === Preloader === */
:root {
  --f7-preloader-modal-padding: 8px;
  --f7-preloader-modal-bg-color: rgba(0, 0, 0, 0.8);
}
.ios {
  --f7-preloader-color: #6c6c6c;
  --f7-preloader-size: 20px;
  --f7-preloader-modal-preloader-size: 34px;
  --f7-preloader-modal-border-radius: 5px;
}
.md {
  --f7-preloader-color: #757575;
  --f7-preloader-size: 32px;
  --f7-preloader-modal-preloader-size: 32px;
  --f7-preloader-modal-border-radius: 4px;
}
.aurora {
  --f7-preloader-color: #757575;
  --f7-preloader-size: 24px;
  --f7-preloader-modal-preloader-size: 24px;
  --f7-preloader-modal-border-radius: 4px;
}
.preloader {
  display: inline-block;
  vertical-align: middle;
  width: var(--f7-preloader-size);
  height: var(--f7-preloader-size);
  font-size: 0;
  position: relative;
}
/* === Preloader Modal === */
.preloader-backdrop {
  visibility: visible;
  opacity: 0;
  background: none;
  z-index: 14000;
}
.preloader-modal {
  position: absolute;
  left: 50%;
  top: 50%;
  padding: var(--f7-preloader-modal-padding);
  background: var(--f7-preloader-modal-bg-color);
  z-index: 14500;
  transform: translateX(-50%) translateY(-50%);
  border-radius: var(--f7-preloader-modal-border-radius);
}
.preloader-modal .preloader {
  --f7-preloader-size: var(--f7-preloader-modal-preloader-size);
  display: block !important;
}
html.with-modal-preloader .page-content {
  overflow: hidden;
  -webkit-overflow-scrolling: auto;
}
.preloader[class*="color-"] {
  --f7-preloader-color: var(--f7-theme-color);
}
.ios .preloader {
  animation: ios-preloader-spin 1s steps(12, end) infinite;
}
.ios .preloader .preloader-inner-line {
  display: block;
  width: 7.15%;
  height: 28.5%;
  border-radius: 100px;
  background: var(--f7-preloader-color);
  position: absolute;
  left: 50%;
  top: 50%;
  transform-origin: center 175%;
}
.ios .preloader .preloader-inner-line:nth-child(1) {
  transform: translate(-50%, -175%) rotate(0deg);
  opacity: 0.27;
}
.ios .preloader .preloader-inner-line:nth-child(2) {
  transform: translate(-50%, -175%) rotate(30deg);
  opacity: 0.32272727;
}
.ios .preloader .preloader-inner-line:nth-child(3) {
  transform: translate(-50%, -175%) rotate(60deg);
  opacity: 0.37545455;
}
.ios .preloader .preloader-inner-line:nth-child(4) {
  transform: translate(-50%, -175%) rotate(90deg);
  opacity: 0.42818182;
}
.ios .preloader .preloader-inner-line:nth-child(5) {
  transform: translate(-50%, -175%) rotate(120deg);
  opacity: 0.48090909;
}
.ios .preloader .preloader-inner-line:nth-child(6) {
  transform: translate(-50%, -175%) rotate(150deg);
  opacity: 0.53363636;
}
.ios .preloader .preloader-inner-line:nth-child(7) {
  transform: translate(-50%, -175%) rotate(180deg);
  opacity: 0.58636364;
}
.ios .preloader .preloader-inner-line:nth-child(8) {
  transform: translate(-50%, -175%) rotate(210deg);
  opacity: 0.63909091;
}
.ios .preloader .preloader-inner-line:nth-child(9) {
  transform: translate(-50%, -175%) rotate(240deg);
  opacity: 0.69181818;
}
.ios .preloader .preloader-inner-line:nth-child(10) {
  transform: translate(-50%, -175%) rotate(270deg);
  opacity: 0.74454545;
}
.ios .preloader .preloader-inner-line:nth-child(11) {
  transform: translate(-50%, -175%) rotate(300deg);
  opacity: 0.79727273;
}
.ios .preloader .preloader-inner-line:nth-child(12) {
  transform: translate(-50%, -175%) rotate(330deg);
  opacity: 0.85;
}
@keyframes ios-preloader-spin {
  100% {
    transform: rotate(360deg);
  }
}
.md .preloader {
  animation: md-preloader-outer 3300ms linear infinite;
}
@keyframes md-preloader-outer {
  0% {
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}
.md .preloader-inner {
  position: relative;
  display: block;
  width: 100%;
  height: 100%;
  animation: md-preloader-inner-rotate 5.25s cubic-bezier(0.35, 0, 0.25, 1) infinite;
}
.md .preloader-inner .preloader-inner-gap {
  position: absolute;
  width: 2px;
  left: 50%;
  margin-left: -1px;
  top: 0;
  bottom: 0;
  box-sizing: border-box;
  border-top: 4px solid var(--f7-preloader-color);
}
.md .preloader-inner .preloader-inner-left,
.md .preloader-inner .preloader-inner-right {
  position: absolute;
  top: 0;
  height: 100%;
  width: 50%;
  overflow: hidden;
}
.md .preloader-inner .preloader-inner-half-circle {
  position: absolute;
  top: 0;
  height: 100%;
  width: 200%;
  box-sizing: border-box;
  border: 4px solid var(--f7-preloader-color);
  border-bottom-color: transparent !important;
  border-radius: 50%;
  animation-iteration-count: infinite;
  animation-duration: 1.3125s;
  animation-timing-function: cubic-bezier(0.35, 0, 0.25, 1);
}
.md .preloader-inner .preloader-inner-left {
  left: 0;
}
.md .preloader-inner .preloader-inner-left .preloader-inner-half-circle {
  left: 0;
  border-right-color: transparent !important;
  animation-name: md-preloader-left-rotate;
}
.md .preloader-inner .preloader-inner-right {
  right: 0;
}
.md .preloader-inner .preloader-inner-right .preloader-inner-half-circle {
  right: 0;
  border-left-color: transparent !important;
  animation-name: md-preloader-right-rotate;
}
.md .preloader.color-multi .preloader-inner-left .preloader-inner-half-circle {
  animation-name: md-preloader-left-rotate-multicolor;
}
.md .preloader.color-multi .preloader-inner-right .preloader-inner-half-circle {
  animation-name: md-preloader-right-rotate-multicolor;
}
@keyframes md-preloader-left-rotate {
  0%,
  100% {
    transform: rotate(130deg);
  }
  50% {
    transform: rotate(-5deg);
  }
}
@keyframes md-preloader-right-rotate {
  0%,
  100% {
    transform: rotate(-130deg);
  }
  50% {
    transform: rotate(5deg);
  }
}
@keyframes md-preloader-inner-rotate {
  12.5% {
    transform: rotate(135deg);
  }
  25% {
    transform: rotate(270deg);
  }
  37.5% {
    transform: rotate(405deg);
  }
  50% {
    transform: rotate(540deg);
  }
  62.5% {
    transform: rotate(675deg);
  }
  75% {
    transform: rotate(810deg);
  }
  87.5% {
    transform: rotate(945deg);
  }
  100% {
    transform: rotate(1080deg);
  }
}
@keyframes md-preloader-left-rotate-multicolor {
  0%,
  100% {
    border-left-color: #4285F4;
    transform: rotate(130deg);
  }
  75% {
    border-left-color: #1B9A59;
    border-top-color: #1B9A59;
  }
  50% {
    border-left-color: #F7C223;
    border-top-color: #F7C223;
    transform: rotate(-5deg);
  }
  25% {
    border-left-color: #DE3E35;
    border-top-color: #DE3E35;
  }
}
@keyframes md-preloader-right-rotate-multicolor {
  0%,
  100% {
    border-right-color: #4285F4;
    transform: rotate(-130deg);
  }
  75% {
    border-right-color: #1B9A59;
    border-top-color: #1B9A59;
  }
  50% {
    border-right-color: #F7C223;
    border-top-color: #F7C223;
    transform: rotate(5deg);
  }
  25% {
    border-top-color: #DE3E35;
    border-right-color: #DE3E35;
  }
}
.aurora .preloader-inner {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
.aurora .preloader-inner-circle {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  border-radius: 50%;
  border: calc(var(--f7-preloader-size) / 8) solid var(--f7-preloader-color);
  border-top-color: transparent;
  box-sizing: border-box;
  animation: aurora-preloader-rotate 1s linear infinite;
}
.aurora .preloader.color-multi .preloader-inner-circle {
  animation: aurora-preloader-rotate 1s linear infinite, aurora-preloader-multicolor 2s linear infinite;
}
@keyframes aurora-preloader-rotate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
@keyframes aurora-preloader-multicolor {
  0%,
  100% {
    border-color: #2196f3;
    border-top-color: transparent;
  }
  25% {
    border-color: #ff3b30;
    border-top-color: transparent;
  }
  50% {
    border-color: #4cd964;
    border-top-color: transparent;
  }
  75% {
    border-color: #ff9500;
    border-top-color: transparent;
  }
}
/* === Progressbar === */
:root {
  /*
  --f7-progressbar-progress-color: var(--f7-theme-color);
  */
}
.ios {
  --f7-progressbar-height: 2px;
  --f7-progressbar-border-radius: 2px;
  --f7-progressbar-bg-color: rgba(0, 0, 0, 0.3);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-progressbar-bg-color: rgba(255, 255, 255, 0.3);
}
.md {
  /*
  --f7-progressbar-bg-color: rgba(var(--f7-theme-color-rgb), 0.5);
  */
  --f7-progressbar-height: 4px;
  --f7-progressbar-border-radius: 0px;
}
.aurora {
  --f7-progressbar-height: 6px;
  --f7-progressbar-border-radius: 3px;
  --f7-progressbar-bg-color: #dbdbdb;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-progressbar-bg-color: #444;
}
.progressbar,
.progressbar-infinite {
  width: 100%;
  overflow: hidden;
  position: relative;
  display: block;
  transform-style: preserve-3d;
  background: var(--f7-progressbar-bg-color, rgba(var(--f7-theme-color-rgb), 0.5));
  transform-origin: center top;
  height: var(--f7-progressbar-height);
  border-radius: var(--f7-progressbar-border-radius);
}
.progressbar {
  vertical-align: middle;
}
.progressbar span {
  background-color: var(--f7-progressbar-progress-color, var(--f7-theme-color));
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  transform: translate3d(-100%, 0, 0);
  transition-duration: 150ms;
}
.progressbar-infinite {
  z-index: 15000;
}
.progressbar-infinite:before,
.progressbar-infinite:after {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  transform-origin: left center;
  transform: translate3d(0, 0, 0);
  display: block;
  background-color: var(--f7-progressbar-progress-color, var(--f7-theme-color));
}
.progressbar-infinite.color-multi {
  background: none !important;
}
.progressbar-in {
  animation: progressbar-in 150ms forwards;
}
.progressbar-out {
  animation: progressbar-out 150ms forwards;
}
body > .progressbar,
.view > .progressbar,
.views > .progressbar,
.page > .progressbar,
.panel > .progressbar,
.popup > .progressbar,
.framework7-root > .progressbar,
body > .progressbar-infinite,
.view > .progressbar-infinite,
.views > .progressbar-infinite,
.page > .progressbar-infinite,
.panel > .progressbar-infinite,
.popup > .progressbar-infinite,
.framework7-root > .progressbar-infinite {
  position: absolute;
  left: 0;
  top: 0;
  z-index: 15000;
  border-radius: 0 !important;
  transform-origin: center top !important;
}
@keyframes progressbar-in {
  from {
    opacity: 0;
    transform: scaleY(0);
  }
  to {
    opacity: 1;
    transform: scaleY(1);
  }
}
@keyframes progressbar-out {
  from {
    opacity: 1;
    transform: scaleY(1);
  }
  to {
    opacity: 0;
    transform: scaleY(0);
  }
}
.ios .progressbar-infinite:before {
  animation: ios-progressbar-infinite 1s linear infinite;
}
.ios .progressbar-infinite:after {
  display: none;
}
.ios .progressbar-infinite.color-multi:before {
  width: 400%;
  background-image: linear-gradient(to right, #4cd964, #5ac8fa, #007aff, #34aadc, #5856d6, #ff2d55, #5856d6, #34aadc, #007aff, #5ac8fa, #4cd964);
  background-size: 25% 100%;
  background-repeat: repeat-x;
  animation: ios-progressbar-infinite-multicolor 3s linear infinite;
}
@keyframes ios-progressbar-infinite {
  0% {
    transform: translate3d(-100%, 0, 0);
  }
  100% {
    transform: translate3d(100%, 0, 0);
  }
}
@keyframes ios-progressbar-infinite-multicolor {
  0% {
    transform: translate3d(0%, 0, 0);
  }
  100% {
    transform: translate3d(-50%, 0, 0);
  }
}
.md .progressbar-infinite:before {
  animation: md-progressbar-infinite-1 2s linear infinite;
}
.md .progressbar-infinite:after {
  animation: md-progressbar-infinite-2 2s linear infinite;
}
.md .progressbar-infinite.color-multi:before {
  background: none;
  animation: md-progressbar-infinite-multicolor-bg 3s step-end infinite;
}
.md .progressbar-infinite.color-multi:after {
  background: none;
  animation: md-progressbar-infinite-multicolor-fill 3s linear infinite;
  transform-origin: center center;
}
@keyframes md-progressbar-infinite-1 {
  0% {
    transform: translateX(-10%) scaleX(0.1);
  }
  25% {
    transform: translateX(30%) scaleX(0.6);
  }
  50% {
    transform: translateX(100%) scaleX(1);
  }
  100% {
    transform: translateX(100%) scaleX(1);
  }
}
@keyframes md-progressbar-infinite-2 {
  0% {
    transform: translateX(-100%) scaleX(1);
  }
  40% {
    transform: translateX(-100%) scaleX(1);
  }
  75% {
    transform: translateX(60%) scaleX(0.35);
  }
  90% {
    transform: translateX(100%) scaleX(0.1);
  }
  100% {
    transform: translateX(100%) scaleX(0.1);
  }
}
@keyframes md-progressbar-infinite-multicolor-bg {
  0% {
    background-color: #4caf50;
  }
  25% {
    background-color: #f44336;
  }
  50% {
    background-color: #2196f3;
  }
  75% {
    background-color: #ffeb3b;
  }
}
@keyframes md-progressbar-infinite-multicolor-fill {
  0% {
    transform: scaleX(0);
    background-color: #f44336;
  }
  24.9% {
    transform: scaleX(1);
    background-color: #f44336;
  }
  25% {
    transform: scaleX(0);
    background-color: #2196f3;
  }
  49.9% {
    transform: scaleX(1);
    background-color: #2196f3;
  }
  50% {
    transform: scaleX(0);
    background-color: #ffeb3b;
  }
  74.9% {
    transform: scaleX(1);
    background-color: #ffeb3b;
  }
  75% {
    transform: scaleX(0);
    background-color: #4caf50;
  }
  100% {
    transform: scaleX(1);
    background-color: #4caf50;
  }
}
.aurora .progressbar,
.aurora .progressbar-infinite,
.aurora .progressbar span,
.aurora .progressbar-infinite:before {
  box-shadow: 0px 0px 0px 1px rgba(0, 0, 0, 0.05) inset;
}
.aurora .progressbar-infinite:before {
  animation: aurora-progressbar-infinite 1s linear infinite;
}
.aurora .progressbar-infinite:after {
  display: none;
}
.aurora .progressbar-infinite.color-multi:before {
  width: 400%;
  background-image: linear-gradient(to right, #4cd964, #5ac8fa, #007aff, #34aadc, #5856d6, #ff2d55, #5856d6, #34aadc, #007aff, #5ac8fa, #4cd964);
  background-size: 25% 100%;
  background-repeat: repeat-x;
  animation: aurora-progressbar-infinite-multicolor 3s linear infinite;
}
@keyframes aurora-progressbar-infinite {
  0% {
    transform: translate3d(-100%, 0, 0);
  }
  100% {
    transform: translate3d(100%, 0, 0);
  }
}
@keyframes aurora-progressbar-infinite-multicolor {
  0% {
    transform: translate3d(0%, 0, 0);
  }
  100% {
    transform: translate3d(-50%, 0, 0);
  }
}
/* === Sortable === */
:root {
  --f7-sortable-handler-color: rgba(0, 0, 0, 0.22);
  --f7-sortable-sorting-item-bg-color: rgba(255, 255, 255, 0.8);
}
:root .theme-dark,
:root.theme-dark {
  --f7-sortable-sorting-item-bg-color: rgba(50, 50, 50, 0.8);
  --f7-sortable-handler-color: rgba(255, 255, 255, 0.55);
}
.ios {
  --f7-sortable-handler-width: 36px;
  --f7-sortable-sorting-item-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.6);
}
.md {
  --f7-sortable-handler-width: 42px;
  --f7-sortable-sorting-item-box-shadow: var(--f7-elevation-2);
}
.aurora {
  --f7-sortable-handler-width: 32px;
  --f7-sortable-sorting-item-box-shadow: var(--f7-elevation-2);
}
.sortable .sortable-handler {
  width: var(--f7-sortable-handler-width);
  height: 100%;
  position: absolute;
  top: 0;
  z-index: 10;
  opacity: 0;
  pointer-events: none;
  cursor: move;
  transition-duration: 300ms;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  right: var(--f7-safe-area-right);
}
.sortable .sortable-handler:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  transition-duration: 300ms;
  transform: translateX(10px);
  color: var(--f7-sortable-handler-color);
  overflow: hidden;
  height: 20px;
  width: 18px;
}
.sortable .item-inner {
  transition-duration: 300ms;
}
.sortable li.sorting {
  z-index: 50;
  background: var(--f7-sortable-sorting-item-bg-color);
  transition-duration: 0ms;
  box-shadow: var(--f7-sortable-sorting-item-box-shadow);
}
.sortable li.sorting .item-inner:after {
  display: none !important;
}
.sortable-sorting li {
  transition-duration: 300ms;
}
.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .sortable-handler {
  pointer-events: auto;
  opacity: 1;
}
.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .sortable-handler:after {
  transform: translateX(0px);
}
.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .item-link .item-inner,
.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .item-link .item-title-row {
  background-image: none !important;
}
.list.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .item-inner,
.list.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .item-link .item-inner,
.list.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .item-link.no-chevron .item-inner,
.list.sortable-enabled.no-chevron li:not(.no-sorting):not(.disallow-sorting) .item-link .item-inner,
.list.sortable-enabled .no-chevron .item-link .item-inner,
.no-chevron .list.sortable-enabled li:not(.no-sorting):not(.disallow-sorting) .item-link .item-inner {
  padding-right: calc(var(--f7-sortable-handler-width) + var(--f7-safe-area-right));
}
.ios .sortable-handler:after {
  content: 'sort_ios';
}
.md .sortable-handler:after {
  content: 'sort_md';
}
.aurora .sortable-handler:after {
  content: 'sort_md';
  font-size: 16px;
  height: 16px;
}
/* === Swipeout === */
:root {
  --f7-swipeout-button-text-color: #fff;
  --f7-swipeout-delete-button-bg-color: #ff3b30;
  --f7-swipeout-button-font-size: inherit;
  --f7-swipeout-button-font-weight: inherit;
  --f7-swipeout-button-bg-color: rgba(0, 0, 0, 0.22);
}
:root .theme-dark,
:root.theme-dark {
  --f7-swipeout-button-bg-color: rgba(255, 255, 255, 0.55);
}
.ios {
  --f7-swipeout-button-padding: 0 30px;
}
.md {
  --f7-swipeout-button-padding: 0 24px;
}
.aurora {
  --f7-swipeout-button-padding: 0 12px;
  --f7-swipeout-button-font-weight: 500;
}
.swipeout {
  overflow: hidden;
  transform-style: preserve-3d;
}
.swipeout-deleting {
  transition-duration: 300ms;
}
.swipeout-deleting .swipeout-content {
  transform: translateX(-100%);
}
.swipeout-transitioning .swipeout-content,
.swipeout-transitioning .swipeout-actions-right a,
.swipeout-transitioning .swipeout-actions-left a,
.swipeout-transitioning .swipeout-overswipe {
  transition-duration: 300ms;
  transition-property: transform, left;
}
.swipeout-content {
  position: relative;
  z-index: 10;
}
.swipeout-overswipe {
  transition-duration: 200ms;
  transition-property: left;
}
.swipeout-actions-left,
.swipeout-actions-right {
  position: absolute;
  top: 0;
  height: 100%;
  display: flex;
  direction: ltr;
}
.swipeout-actions-left > a,
.swipeout-actions-right > a,
.swipeout-actions-left > button,
.swipeout-actions-right > button,
.swipeout-actions-left > span,
.swipeout-actions-right > span,
.swipeout-actions-left > div,
.swipeout-actions-right > div {
  color: var(--f7-swipeout-button-text-color);
  background: var(--f7-swipeout-button-bg-color);
  padding: var(--f7-swipeout-button-padding);
  display: flex;
  align-items: center;
  position: relative;
  left: 0;
  font-size: var(--f7-swipeout-button-font-size);
  font-weight: var(--f7-swipeout-button-font-weight);
}
.swipeout-actions-left > a:after,
.swipeout-actions-right > a:after,
.swipeout-actions-left > button:after,
.swipeout-actions-right > button:after,
.swipeout-actions-left > span:after,
.swipeout-actions-right > span:after,
.swipeout-actions-left > div:after,
.swipeout-actions-right > div:after {
  content: '';
  position: absolute;
  top: 0;
  width: 600%;
  height: 100%;
  background: inherit;
  z-index: -1;
  transform: translate3d(0, 0, 0);
  pointer-events: none;
}
.swipeout-actions-left .swipeout-delete,
.swipeout-actions-right .swipeout-delete {
  background: var(--f7-swipeout-delete-button-bg-color);
}
.swipeout-actions-right {
  right: 0%;
  transform: translateX(100%);
}
.swipeout-actions-right > a:after,
.swipeout-actions-right > button:after,
.swipeout-actions-right > span:after,
.swipeout-actions-right > div:after {
  left: 100%;
  margin-left: -1px;
}
.swipeout-actions-left {
  left: 0%;
  transform: translateX(-100%);
}
.swipeout-actions-left > a:after,
.swipeout-actions-left > button:after,
.swipeout-actions-left > span:after,
.swipeout-actions-left > div:after {
  right: 100%;
  margin-right: -1px;
}
.swipeout-actions-left [class*="color-"],
.swipeout-actions-right [class*="color-"] {
  --f7-swipeout-button-bg-color: var(--f7-theme-color);
}
/* === Accordion === */
.accordion-item-toggle {
  cursor: pointer;
  transition-duration: 300ms;
}
.accordion-item-toggle.active-state {
  transition-duration: 300ms;
}
.accordion-item-toggle.active-state > .item-inner:after {
  background-color: transparent;
}
.accordion-item-toggle .item-inner {
  transition-duration: 300ms;
  transition-property: background-color;
}
.accordion-item-toggle .item-inner:after {
  transition-duration: 300ms;
}
.accordion-item .item-link .item-inner:after {
  transition-duration: 300ms;
}
.accordion-item .list,
.accordion-item .block {
  margin-top: 0;
  margin-bottom: 0;
}
.accordion-item .block > h1:first-child,
.accordion-item .block > h2:first-child,
.accordion-item .block > h3:first-child,
.accordion-item .block > h4:first-child,
.accordion-item .block > p:first-child {
  margin-top: 10px;
}
.accordion-item .block > h1:last-child,
.accordion-item .block > h2:last-child,
.accordion-item .block > h3:last-child,
.accordion-item .block > h4:last-child,
.accordion-item .block > p:last-child {
  margin-bottom: 10px;
}
.accordion-item-opened .accordion-item-toggle .item-inner:after,
.accordion-item-opened > .item-link .item-inner:after {
  background-color: transparent;
}
.list li.accordion-item ul {
  padding-left: 0;
}
.accordion-item-content {
  position: relative;
  overflow: hidden;
  height: 0;
  font-size: 14px;
  transition-duration: 300ms;
}
.accordion-item-opened > .accordion-item-content {
  height: auto;
}
html.device-android-4 .accordion-item-content {
  transform: none;
}
.list .accordion-item-toggle .item-inner {
  padding-right: calc(var(--f7-list-chevron-icon-area) + var(--f7-safe-area-right));
}
.list .accordion-item-toggle .item-inner:before {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 50%;
  width: 14px;
  height: 8px;
  margin-top: -4px;
  font-size: 20px;
  line-height: 14px;
  color: var(--f7-list-chevron-icon-color);
  pointer-events: none;
  right: calc(var(--f7-list-item-padding-horizontal) + var(--f7-safe-area-right));
  content: 'chevron_right';
}
.list .accordion-item-toggle.active-state {
  background-color: var(--f7-list-link-pressed-bg-color);
}
.list .accordion-item-toggle .item-inner:before,
.list:not(.media-list) .accordion-item:not(.media-item) .accordion-item-toggle .item-inner:before,
.list:not(.media-list) .accordion-item:not(.media-item) > .item-link .item-inner:before,
.media-list .accordion-item .accordion-item-toggle .item-title-row:before,
.media-list .accordion-item > .item-link .item-title-row:before,
.accordion-item.media-item .accordion-item-toggle .item-title-row:before,
.accordion-item.media-item > .item-link .item-title-row:before,
.links-list .accordion-item > a:before {
  content: 'chevron_down';
  width: 14px;
  height: 8px;
  margin-top: -4px;
  line-height: 8px;
}
.list .accordion-item-toggle.accordion-item-opened .item-inner:before,
.list:not(.media-list) .accordion-item-opened:not(.media-item) .accordion-item-toggle .item-inner:before,
.list:not(.media-list) .accordion-item-opened:not(.media-item) > .item-link .item-inner:before,
.media-list .accordion-item-opened .accordion-item-toggle .item-title-row:before,
.media-list .accordion-item-opened > .item-link .item-title-row:before,
.accordion-item-opened.media-item .accordion-item-toggle .item-title-row:before,
.accordion-item-opened.media-item > .item-link .item-title-row:before,
.links-list .accordion-item-opened > a:before {
  content: 'chevron_up';
  width: 14px;
  height: 8px;
  margin-top: -4px;
  line-height: 8px;
}
.aurora .list .accordion-item-toggle .item-inner:before,
.aurora .list:not(.media-list) .accordion-item:not(.media-item) .accordion-item-toggle .item-inner:before,
.aurora .list:not(.media-list) .accordion-item:not(.media-item) > .item-link .item-inner:before,
.aurora .media-list .accordion-item .accordion-item-toggle .item-title-row:before,
.aurora .media-list .accordion-item > .item-link .item-title-row:before,
.aurora .accordion-item.media-item .accordion-item-toggle .item-title-row:before,
.aurora .accordion-item.media-item > .item-link .item-title-row:before,
.aurora .links-list .accordion-item > a:before {
  content: 'chevron_down_aurora';
}
.aurora .list .accordion-item-toggle.accordion-item-opened .item-inner:before,
.aurora .list:not(.media-list) .accordion-item-opened:not(.media-item) .accordion-item-toggle .item-inner:before,
.aurora .list:not(.media-list) .accordion-item-opened:not(.media-item) > .item-link .item-inner:before,
.aurora .media-list .accordion-item-opened .accordion-item-toggle .item-title-row:before,
.aurora .media-list .accordion-item-opened > .item-link .item-title-row:before,
.aurora .accordion-item-opened.media-item .accordion-item-toggle .item-title-row:before,
.aurora .accordion-item-opened.media-item > .item-link .item-title-row:before,
.aurora .links-list .accordion-item-opened > a:before {
  content: 'chevron_up_aurora';
}
/* === Contacts === */
:root .theme-dark,
:root.theme-dark {
  --f7-contacts-list-title-text-color: #fff;
}
.ios {
  --f7-contacts-list-title-font-size: inherit;
  --f7-contacts-list-title-font-weight: 600;
  --f7-contacts-list-title-height: 22px;
  --f7-contacts-list-title-text-color: #000;
  --f7-contacts-list-title-bg-color: #f7f7f7;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-contacts-list-title-bg-color: #323234;
}
.md {
  --f7-contacts-list-title-font-size: 20px;
  --f7-contacts-list-title-font-weight: 500;
  /*
  --f7-contacts-list-title-text-color: var(--f7-theme-color);
  */
  --f7-contacts-list-title-height: 48px;
  --f7-contacts-list-title-bg-color: transparent;
}
.aurora {
  --f7-contacts-list-title-font-weight: 600;
  --f7-contacts-list-title-text-color: #000;
  /*
  --f7-contacts-list-title-bg-color: var(--f7-list-group-title-bg-color);
  --f7-contacts-list-title-font-size: var(--f7-list-group-title-font-size);
  --f7-contacts-list-title-line-height: var(--f7-list-group-title-height);
  --f7-contacts-list-title-height: var(--f7-list-group-title-height);
  */
}
.contacts-list {
  --f7-list-margin-vertical: 0px;
}
.contacts-list .list-group-title,
.contacts-list li.list-group-title {
  background-color: var(--f7-contacts-list-title-bg-color, var(--f7-list-group-title-bg-color));
  font-weight: var(--f7-contacts-list-title-font-weight, var(--f7-list-group-title-font-weight));
  font-size: var(--f7-contacts-list-title-font-size, var(--f7-list-group-title-font-size));
  color: var(--f7-contacts-list-title-text-color, var(--f7-theme-color));
  line-height: var(--f7-contacts-list-title-height, var(--f7-list-group-title-height));
  height: var(--f7-contacts-list-title-height, var(--f7-list-group-title-height));
}
.contacts-list .list-group:first-child ul:before {
  display: none !important;
}
.contacts-list .list-group:last-child ul:after {
  display: none !important;
}
.md .contacts-list .list-group-title {
  pointer-events: none;
  overflow: visible;
  width: 56px;
}
.md .contacts-list .list-group-title + li {
  margin-top: calc(var(--f7-contacts-list-title-height) * -1);
}
.md .contacts-list li:not(.list-group-title) {
  padding-left: 56px;
}
/* === Virtual List === */
/* === Indexed List === */
:root {
  --f7-list-index-width: 16px;
  --f7-list-index-font-size: 11px;
  --f7-list-index-font-weight: 600;
  /* --f7-list-index-text-color: var(--f7-theme-color); */
  --f7-list-index-item-height: 14px;
  --f7-list-index-label-text-color: #fff;
  /* --f7-list-index-label-bg-color: var(--f7-theme-color); */
  --f7-list-index-label-font-weight: 500;
}
.ios {
  --f7-list-index-label-size: 44px;
  --f7-list-index-label-font-size: 17px;
  --f7-list-index-skip-dot-size: 6px;
}
.md {
  --f7-list-index-label-size: 56px;
  --f7-list-index-label-font-size: 20px;
  --f7-list-index-skip-dot-size: 4px;
}
.aurora {
  --f7-list-index-font-size: 12px;
  --f7-list-index-label-size: 32px;
  --f7-list-index-label-font-size: 12px;
  --f7-list-index-label-font-weight: 600;
  --f7-list-index-skip-dot-size: 4px;
}
.list-index {
  position: absolute;
  top: 0;
  bottom: 0;
  text-align: center;
  z-index: 10;
  width: var(--f7-list-index-width);
  cursor: pointer;
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
  right: var(--f7-safe-area-right);
}
.list-index:before {
  content: '';
  position: absolute;
  width: 20px;
  top: 0;
  right: 100%;
  height: 100%;
}
.list-index ul {
  color: var(--f7-list-index-text-color, var(--f7-theme-color));
  font-size: var(--f7-list-index-font-size);
  font-weight: var(--f7-list-index-font-weight);
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  height: 100%;
  width: 100%;
  position: relative;
}
.list-index li {
  margin: 0;
  padding: 0;
  list-style: none;
  position: relative;
  height: var(--f7-list-index-item-height);
  line-height: var(--f7-list-index-item-height);
  flex-shrink: 0;
  display: block;
  width: 100%;
}
.list-index .list-index-skip-placeholder:after {
  content: '';
  position: absolute;
  left: 50%;
  top: 50%;
  border-radius: 50%;
  width: var(--f7-list-index-skip-dot-size);
  height: var(--f7-list-index-skip-dot-size);
  margin-left: calc(-1 * var(--f7-list-index-skip-dot-size) / 2);
  margin-top: calc(-1 * var(--f7-list-index-skip-dot-size) / 2);
  background: var(--f7-list-index-text-color, var(--f7-theme-color));
}
.list-index .list-index-label {
  position: absolute;
  bottom: 0;
  right: 100%;
  text-align: center;
  background-color: var(--f7-list-index-label-bg-color, var(--f7-theme-color));
  color: var(--f7-list-index-label-text-color);
  width: var(--f7-list-index-label-size);
  height: var(--f7-list-index-label-size);
  line-height: var(--f7-list-index-label-size);
  font-size: var(--f7-list-index-label-font-size);
  font-weight: var(--f7-list-index-label-font-weight);
}
.navbar ~ .page > .list-index,
.navbars ~ .page > .list-index,
.navbar ~ .list-index {
  top: var(--f7-navbar-height);
}
.navbar ~ .toolbar-top ~ .list-index,
.navbars ~ .toolbar-top ~ .list-index,
.ios .navbar ~ .toolbar-top-ios ~ .list-index,
.ios .navbars ~ .toolbar-top-ios .md .navbar ~ .toolbar-top-md ~ .list-index {
  top: calc(var(--f7-navbar-height) + var(--f7-toolbar-height));
}
.navbar ~ .toolbar-top.tabbar-labels ~ .list-index,
.navbars ~ .toolbar-top.tabbar-labels ~ .list-index,
.ios .navbar ~ .toolbar-top-ios.tabbar-labels ~ .list-index,
.ios .navbars ~ .toolbar-top-ios .md .navbar ~ .toolbar-top-md.tabbar-labels ~ .list-index {
  top: calc(var(--f7-navbar-height) + var(--f7-tabbar-labels-height));
}
.navbar ~ .subnavbar ~ .list-index,
.navbars ~ .subnavbar ~ .list-index,
.page-with-subnavbar .navbar ~ .list-index {
  top: calc(var(--f7-navbar-height) + var(--f7-subnavbar-height));
}
.toolbar-bottom ~ .page > .list-index,
.ios .toolbar-bottom-ios ~ .page > .list-index,
.md .toolbar-bottom-md ~ .page > .list-index,
.toolbar-bottom ~ * .page > .list-index,
.ios .toolbar-bottom-ios ~ * .page > .list-index,
.md .toolbar-bottom-md ~ * .page > .list-index,
.toolbar-bottom ~ .list-index,
.ios .toolbar-bottom-ios ~ .list-index,
.md .toolbar-bottom-md ~ .list-index {
  bottom: calc(var(--f7-toolbar-height) + var(--f7-safe-area-bottom));
}
.toolbar-bottom.tabbar-labels ~ .page > .list-index,
.ios .toolbar-bottom-ios.tabbar-labels ~ .page > .list-index,
.md .toolbar-bottom-md.tabbar-labels ~ .page > .list-index,
.toolbar-bottom.tabbar-labels ~ * .page > .list-index,
.ios .toolbar-bottom-ios.tabbar-labels ~ * .page > .list-index,
.md .toolbar-bottom-md.tabbar-labels ~ * .page > .list-index,
.toolbar-bottom.tabbar-labels ~ .list-index,
.ios .toolbar-bottom-ios.tabbar-labels ~ .list-index,
.md .toolbar-bottom-md.tabbar-labels ~ .list-index {
  bottom: calc(var(--f7-tabbar-labels-height) + var(--f7-safe-area-bottom));
}
.ios .list-index .list-index-label {
  margin-bottom: calc(-1 * var(--f7-list-index-label-size) / 2);
  margin-right: calc(var(--f7-list-index-width) - 1px);
  border-radius: 50%;
}
.ios .list-index .list-index-label:before {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50% 0% 50% 50%;
  content: '';
  background-color: inherit;
  left: 0;
  top: 0;
  transform: rotate(45deg);
  z-index: -1;
}
.md .list-index .list-index-label {
  border-radius: 50% 50% 0 50%;
}
.aurora .list-index .list-index-label {
  margin-bottom: calc(-1 * var(--f7-list-index-label-size) / 2);
  margin-right: calc(var(--f7-list-index-width) - 1px);
  border-radius: 50%;
}
.aurora .list-index .list-index-label:before {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50% 1px 50% 50%;
  content: '';
  background-color: inherit;
  left: 0;
  top: 0;
  transform: rotate(45deg);
  z-index: -1;
}
/* === Timeline === */
:root {
  --f7-timeline-inner-block-margin-vertical: 16px;
  --f7-timeline-divider-margin-horizontal: 16px;
  --f7-timeline-horizontal-date-height: 34px;
  --f7-timeline-year-height: 24px;
  --f7-timeline-year-font-weight: inherit;
  --f7-timeline-month-height: 24px;
  --f7-timeline-month-font-size: inherit;
  --f7-timeline-month-font-weight: inherit;
  --f7-timeline-item-text-font-weight: inherit;
  --f7-timeline-item-subtitle-font-weight: inherit;
  --f7-timeline-item-inner-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-timeline-item-inner-bg-color: #1c1c1d;
  --f7-timeline-horizontal-item-border-color: rgba(255, 255, 255, 0.15);
  --f7-timeline-horizontal-item-date-border-color: rgba(255, 255, 255, 0.15);
}
.ios {
  --f7-timeline-padding-horizontal: 16px;
  --f7-timeline-margin-vertical: 35px;
  --f7-timeline-item-inner-border-radius: 7px;
  --f7-timeline-item-inner-box-shadow: none;
  --f7-timeline-item-time-font-size: 13px;
  --f7-timeline-item-title-font-size: 17px;
  --f7-timeline-item-title-line-height: inherit;
  --f7-timeline-item-title-font-weight: 600;
  --f7-timeline-item-subtitle-font-size: 15px;
  --f7-timeline-item-subtitle-line-height: inherit;
  --f7-timeline-item-text-font-size: inherit;
  --f7-timeline-item-text-color: inherit;
  --f7-timeline-item-text-line-height: inherit;
  --f7-timeline-year-font-size: 16px;
  --f7-timeline-horizontal-item-padding: 10px;
  --f7-timeline-horizontal-item-date-shadow-image: none;
  --f7-timeline-item-time-text-color: rgba(0, 0, 0, 0.45);
  --f7-timeline-horizontal-item-border-color: rgba(0, 0, 0, 0.22);
  --f7-timeline-horizontal-item-date-border-color: rgba(0, 0, 0, 0.22);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-timeline-item-time-text-color: rgba(255, 255, 255, 0.55);
}
.md {
  --f7-timeline-padding-horizontal: 16px;
  --f7-timeline-margin-vertical: 32px;
  --f7-timeline-item-inner-border-radius: 4px;
  --f7-timeline-item-inner-box-shadow: var(--f7-elevation-1);
  --f7-timeline-item-time-font-size: 13px;
  --f7-timeline-item-title-font-size: 16px;
  --f7-timeline-item-title-line-height: inherit;
  --f7-timeline-item-title-font-weight: 400;
  --f7-timeline-item-subtitle-font-size: inherit;
  --f7-timeline-item-subtitle-line-height: inherit;
  --f7-timeline-item-text-font-size: inherit;
  --f7-timeline-item-text-line-height: inherit;
  --f7-timeline-item-text-color: inherit;
  --f7-timeline-year-font-size: 16px;
  --f7-timeline-horizontal-item-padding: 12px;
  --f7-timeline-horizontal-item-date-shadow-image: var(--f7-bars-shadow-bottom-image);
  --f7-timeline-item-time-text-color: rgba(0, 0, 0, 0.54);
  --f7-timeline-horizontal-item-border-color: rgba(0, 0, 0, 0.12);
  --f7-timeline-horizontal-item-date-border-color: transparent;
}
.md .theme-dark,
.md.theme-dark {
  --f7-timeline-item-time-text-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-timeline-padding-horizontal: 10px;
  --f7-timeline-margin-vertical: 15px;
  --f7-timeline-item-inner-border-radius: 4px;
  --f7-timeline-item-inner-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.15);
  --f7-timeline-item-time-font-size: 12px;
  --f7-timeline-item-title-font-size: 14px;
  --f7-timeline-item-title-line-height: 1.3;
  --f7-timeline-item-title-font-weight: 600;
  --f7-timeline-item-subtitle-font-size: 14px;
  --f7-timeline-item-subtitle-line-height: 1.3;
  --f7-timeline-item-text-font-size: 12px;
  --f7-timeline-item-text-line-height: 1.33;
  --f7-timeline-year-font-size: 14px;
  --f7-timeline-year-font-weight: 500;
  --f7-timeline-horizontal-item-padding: 10px;
  --f7-timeline-horizontal-item-date-shadow-image: none;
  --f7-timeline-item-time-text-color: rgba(0, 0, 0, 0.5);
  --f7-timeline-item-text-color: rgba(0, 0, 0, 0.6);
  --f7-timeline-horizontal-item-border-color: rgba(0, 0, 0, 0.2);
  --f7-timeline-horizontal-item-date-border-color: rgba(0, 0, 0, 0.2);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-timeline-item-time-text-color: rgba(255, 255, 255, 0.54);
  --f7-timeline-item-text-color: rgba(255, 255, 255, 0.54);
}
.timeline {
  box-sizing: border-box;
  margin: var(--f7-timeline-margin-vertical) 0;
  padding: 0 var(--f7-timeline-padding-horizontal);
  padding-top: 0;
  padding-bottom: 0;
  padding-left: calc(var(--f7-timeline-padding-horizontal) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-timeline-padding-horizontal) + var(--f7-safe-area-right));
}
.block-strong .timeline {
  padding: 0;
  margin: 0;
}
.timeline-item {
  display: flex;
  justify-content: flex-start;
  overflow: hidden;
  box-sizing: border-box;
  position: relative;
  padding: 2px 0px var(--f7-timeline-padding-horizontal);
}
.timeline-item:last-child {
  padding-bottom: 2px;
}
.timeline-item-date {
  flex-shrink: 0;
  width: 50px;
  text-align: right;
  box-sizing: border-box;
}
.timeline-item-date small {
  font-size: 10px;
}
.timeline-item-content {
  margin: 2px;
  min-width: 0;
  position: relative;
  flex-shrink: 10;
}
.timeline-item-content .card,
.timeline-item-content.card,
.timeline-item-content .list,
.timeline-item-content.list,
.timeline-item-content .block,
.timeline-item-content.block {
  margin: 0;
  width: 100%;
}
.timeline-item-content .card + .card,
.timeline-item-content .list + .card,
.timeline-item-content .block + .card,
.timeline-item-content .card + .list,
.timeline-item-content .list + .list,
.timeline-item-content .block + .list,
.timeline-item-content .card + .block,
.timeline-item-content .list + .block,
.timeline-item-content .block + .block {
  margin: var(--f7-timeline-inner-block-margin-vertical) 0 0;
}
.timeline-item-content p:first-child,
.timeline-item-content ul:first-child,
.timeline-item-content ol:first-child,
.timeline-item-content h1:first-child,
.timeline-item-content h2:first-child,
.timeline-item-content h3:first-child,
.timeline-item-content h4:first-child {
  margin-top: 0;
}
.timeline-item-content p:last-child,
.timeline-item-content ul:last-child,
.timeline-item-content ol:last-child,
.timeline-item-content h1:last-child,
.timeline-item-content h2:last-child,
.timeline-item-content h3:last-child,
.timeline-item-content h4:last-child {
  margin-bottom: 0;
}
.timeline-item-inner {
  background: var(--f7-timeline-item-inner-bg-color);
  box-sizing: border-box;
  border-radius: var(--f7-timeline-item-inner-border-radius);
  padding: 8px var(--f7-timeline-padding-horizontal);
  box-shadow: var(--f7-timeline-item-inner-box-shadow);
}
.timeline-item-inner + .timeline-item-inner {
  margin-top: var(--f7-timeline-inner-block-margin-vertical);
}
.timeline-item-inner .block {
  padding: 0;
  color: inherit;
}
.timeline-item-inner .block-strong {
  padding-left: 0;
  padding-right: 0;
  margin: 0;
}
.timeline-item-inner .block-strong:before,
.timeline-item-inner .block-strong:after {
  display: none !important;
}
.timeline-item-inner .list ul:before,
.timeline-item-inner .list ul:after {
  display: none !important;
}
.timeline-item-divider {
  width: 1px;
  position: relative;
  width: 10px;
  height: 10px;
  background: #bbb;
  border-radius: 50%;
  flex-shrink: 0;
  margin: 3px var(--f7-timeline-divider-margin-horizontal) 0;
}
.timeline-item-divider:after,
.timeline-item-divider:before {
  content: ' ';
  width: 1px;
  height: 100vh;
  position: absolute;
  left: 50%;
  background: inherit;
  transform: translate3d(-50%, 0, 0);
}
.timeline-item-divider:after {
  top: 100%;
}
.timeline-item-divider:before {
  bottom: 100%;
}
.timeline-item:last-child .timeline-item-divider:after {
  display: none;
}
.timeline-item:first-child .timeline-item-divider:before {
  display: none;
}
.timeline-item-time {
  font-size: var(--f7-timeline-item-time-font-size);
  margin-top: var(--f7-timeline-inner-block-margin-vertical);
  color: var(--f7-timeline-item-time-text-color);
}
.timeline-item-time:first-child,
.timeline-item-time:last-child {
  margin-top: 0;
}
.timeline-item-title + .timeline-item-time {
  margin-top: 0;
}
.timeline-item-title {
  font-size: var(--f7-timeline-item-title-font-size);
  font-weight: var(--f7-timeline-item-title-font-weight);
  line-height: var(--f7-timeline-item-title-line-height);
}
.timeline-item-subtitle {
  font-size: var(--f7-timeline-item-subtitle-font-size);
  font-weight: var(--f7-timeline-item-subtitle-font-weight);
  line-height: var(--f7-timeline-item-subtitle-line-height);
}
.timeline-item-text {
  color: var(--f7-timeline-item-text-color);
  font-size: var(--f7-timeline-item-text-font-size);
  font-weight: var(--f7-timeline-item-text-font-weight);
  line-height: var(--f7-timeline-item-text-line-height);
}
.timeline-sides .timeline-item-right,
.timeline-sides .timeline-item {
  margin-left: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
  margin-right: 0;
}
.timeline-sides .timeline-item-right .timeline-item-date,
.timeline-sides .timeline-item .timeline-item-date {
  text-align: right;
}
.timeline-sides .timeline-item-left,
.timeline-sides .timeline-item:not(.timeline-item-right):nth-child(2n) {
  flex-direction: row-reverse;
  margin-right: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
  margin-left: 0;
}
.timeline-sides .timeline-item-left .timeline-item-date,
.timeline-sides .timeline-item:not(.timeline-item-right):nth-child(2n) .timeline-item-date {
  text-align: left;
}
@media (min-width: 480px) {
  .xsmall-sides .timeline-item-right,
  .xsmall-sides .timeline-item {
    margin-left: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-right: 0;
  }
  .xsmall-sides .timeline-item-right .timeline-item-date,
  .xsmall-sides .timeline-item .timeline-item-date {
    text-align: right;
  }
  .xsmall-sides .timeline-item-left,
  .xsmall-sides .timeline-item:not(.timeline-item-right):nth-child(2n) {
    flex-direction: row-reverse;
    margin-right: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-left: 0;
  }
  .xsmall-sides .timeline-item-left .timeline-item-date,
  .xsmall-sides .timeline-item:not(.timeline-item-right):nth-child(2n) .timeline-item-date {
    text-align: left;
  }
}
@media (min-width: 568px) {
  .small-sides .timeline-item-right,
  .small-sides .timeline-item {
    margin-left: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-right: 0;
  }
  .small-sides .timeline-item-right .timeline-item-date,
  .small-sides .timeline-item .timeline-item-date {
    text-align: right;
  }
  .small-sides .timeline-item-left,
  .small-sides .timeline-item:not(.timeline-item-right):nth-child(2n) {
    flex-direction: row-reverse;
    margin-right: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-left: 0;
  }
  .small-sides .timeline-item-left .timeline-item-date,
  .small-sides .timeline-item:not(.timeline-item-right):nth-child(2n) .timeline-item-date {
    text-align: left;
  }
}
@media (min-width: 768px) {
  .medium-sides .timeline-item-right,
  .medium-sides .timeline-item {
    margin-left: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-right: 0;
  }
  .medium-sides .timeline-item-right .timeline-item-date,
  .medium-sides .timeline-item .timeline-item-date {
    text-align: right;
  }
  .medium-sides .timeline-item-left,
  .medium-sides .timeline-item:not(.timeline-item-right):nth-child(2n) {
    flex-direction: row-reverse;
    margin-right: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-left: 0;
  }
  .medium-sides .timeline-item-left .timeline-item-date,
  .medium-sides .timeline-item:not(.timeline-item-right):nth-child(2n) .timeline-item-date {
    text-align: left;
  }
}
@media (min-width: 1024px) {
  .large-sides .timeline-item-right,
  .large-sides .timeline-item {
    margin-left: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-right: 0;
  }
  .large-sides .timeline-item-right .timeline-item-date,
  .large-sides .timeline-item .timeline-item-date {
    text-align: right;
  }
  .large-sides .timeline-item-left,
  .large-sides .timeline-item:not(.timeline-item-right):nth-child(2n) {
    flex-direction: row-reverse;
    margin-right: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-left: 0;
  }
  .large-sides .timeline-item-left .timeline-item-date,
  .large-sides .timeline-item:not(.timeline-item-right):nth-child(2n) .timeline-item-date {
    text-align: left;
  }
}
@media (min-width: 1200px) {
  .xlarge-sides .timeline-item-right,
  .xlarge-sides .timeline-item {
    margin-left: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-right: 0;
  }
  .xlarge-sides .timeline-item-right .timeline-item-date,
  .xlarge-sides .timeline-item .timeline-item-date {
    text-align: right;
  }
  .xlarge-sides .timeline-item-left,
  .xlarge-sides .timeline-item:not(.timeline-item-right):nth-child(2n) {
    flex-direction: row-reverse;
    margin-right: calc(50% - (var(--f7-timeline-divider-margin-horizontal) * 2 + 10px) / 2 - 50px);
    margin-left: 0;
  }
  .xlarge-sides .timeline-item-left .timeline-item-date,
  .xlarge-sides .timeline-item:not(.timeline-item-right):nth-child(2n) .timeline-item-date {
    text-align: left;
  }
}
.timeline-horizontal {
  height: 100%;
  display: flex;
  padding: 0;
  margin: 0;
  position: relative;
  padding-left: var(--f7-safe-area-left);
  padding-right: 0;
}
.timeline-horizontal .timeline-item {
  display: block;
  width: 33.33333333vw;
  margin: 0;
  padding: 0;
  flex-shrink: 0;
  position: relative;
  height: 100%;
  padding-top: var(--f7-timeline-horizontal-date-height) !important;
  padding-bottom: var(--f7-timeline-horizontal-item-padding);
}
.timeline-horizontal .timeline-item:after {
  content: '';
  position: absolute;
  background-color: var(--f7-timeline-horizontal-item-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: 0;
  bottom: auto;
  left: auto;
  width: 1px;
  height: 100%;
  transform-origin: 100% 50%;
  transform: scaleX(calc(1 / var(--f7-device-pixel-ratio)));
}
.timeline-horizontal .timeline-item-date {
  padding: 0px var(--f7-timeline-horizontal-item-padding);
  width: auto;
  line-height: var(--f7-timeline-horizontal-date-height);
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: var(--f7-timeline-horizontal-date-height);
  background-color: var(--f7-bars-bg-color);
  color: var(--f7-bars-text-color);
  text-align: left;
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .timeline-horizontal .timeline-item-date {
    background-color: rgba(var(--f7-bars-bg-color-rgb), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.timeline-horizontal .timeline-item-date:after {
  content: '';
  position: absolute;
  background-color: var(--f7-timeline-horizontal-item-date-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.timeline-horizontal .timeline-item-date:before {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  top: 100%;
  bottom: auto;
  height: 8px;
  pointer-events: none;
  background: var(--f7-timeline-horizontal-item-date-shadow-image);
}
.timeline-horizontal.no-shadow .timeline-item-date:before {
  display: none;
}
.timeline-horizontal .timeline-item-content {
  padding: var(--f7-timeline-horizontal-item-padding);
  height: calc(100% - var(--f7-timeline-horizontal-item-padding));
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  margin: 0;
}
.timeline-horizontal .timeline-item-divider {
  display: none;
}
.timeline-horizontal > .timeline-item:last-child:after,
.timeline-horizontal .timeline-month:last-child .timeline-item:last-child:after {
  display: none !important;
}
.timeline-horizontal.col-5 .timeline-item {
  width: 5vw;
}
.timeline-horizontal.col-10 .timeline-item {
  width: 10vw;
}
.timeline-horizontal.col-15 .timeline-item {
  width: 15vw;
}
.timeline-horizontal.col-20 .timeline-item {
  width: 20vw;
}
.timeline-horizontal.col-25 .timeline-item {
  width: 25vw;
}
.timeline-horizontal.col-30 .timeline-item {
  width: 30vw;
}
.timeline-horizontal.col-33 .timeline-item {
  width: 33.333333333333336vw;
}
.timeline-horizontal.col-35 .timeline-item {
  width: 35vw;
}
.timeline-horizontal.col-40 .timeline-item {
  width: 40vw;
}
.timeline-horizontal.col-45 .timeline-item {
  width: 45vw;
}
.timeline-horizontal.col-50 .timeline-item {
  width: 50vw;
}
.timeline-horizontal.col-55 .timeline-item {
  width: 55vw;
}
.timeline-horizontal.col-60 .timeline-item {
  width: 60vw;
}
.timeline-horizontal.col-65 .timeline-item {
  width: 65vw;
}
.timeline-horizontal.col-66 .timeline-item {
  width: 66.66666666666666vw;
}
.timeline-horizontal.col-70 .timeline-item {
  width: 70vw;
}
.timeline-horizontal.col-75 .timeline-item {
  width: 75vw;
}
.timeline-horizontal.col-80 .timeline-item {
  width: 80vw;
}
.timeline-horizontal.col-85 .timeline-item {
  width: 85vw;
}
.timeline-horizontal.col-90 .timeline-item {
  width: 90vw;
}
.timeline-horizontal.col-95 .timeline-item {
  width: 95vw;
}
.timeline-horizontal.col-100 .timeline-item {
  width: 100vw;
}
@media (min-width: 768px) {
  .timeline-horizontal.tablet-5 .timeline-item {
    width: 5vw;
  }
  .timeline-horizontal.tablet-10 .timeline-item {
    width: 10vw;
  }
  .timeline-horizontal.tablet-15 .timeline-item {
    width: 15vw;
  }
  .timeline-horizontal.tablet-20 .timeline-item {
    width: 20vw;
  }
  .timeline-horizontal.tablet-25 .timeline-item {
    width: 25vw;
  }
  .timeline-horizontal.tablet-30 .timeline-item {
    width: 30vw;
  }
  .timeline-horizontal.tablet-33 .timeline-item {
    width: 33.333333333333336vw;
  }
  .timeline-horizontal.tablet-35 .timeline-item {
    width: 35vw;
  }
  .timeline-horizontal.tablet-40 .timeline-item {
    width: 40vw;
  }
  .timeline-horizontal.tablet-45 .timeline-item {
    width: 45vw;
  }
  .timeline-horizontal.tablet-50 .timeline-item {
    width: 50vw;
  }
  .timeline-horizontal.tablet-55 .timeline-item {
    width: 55vw;
  }
  .timeline-horizontal.tablet-60 .timeline-item {
    width: 60vw;
  }
  .timeline-horizontal.tablet-65 .timeline-item {
    width: 65vw;
  }
  .timeline-horizontal.tablet-66 .timeline-item {
    width: 66.66666666666666vw;
  }
  .timeline-horizontal.tablet-70 .timeline-item {
    width: 70vw;
  }
  .timeline-horizontal.tablet-75 .timeline-item {
    width: 75vw;
  }
  .timeline-horizontal.tablet-80 .timeline-item {
    width: 80vw;
  }
  .timeline-horizontal.tablet-85 .timeline-item {
    width: 85vw;
  }
  .timeline-horizontal.tablet-90 .timeline-item {
    width: 90vw;
  }
  .timeline-horizontal.tablet-95 .timeline-item {
    width: 95vw;
  }
  .timeline-horizontal.tablet-100 .timeline-item {
    width: 100vw;
  }
}
.timeline-year {
  padding-top: var(--f7-timeline-year-height);
}
.timeline-year:after {
  content: '';
  position: absolute;
  background-color: var(--f7-timeline-horizontal-item-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: 0;
  bottom: auto;
  left: auto;
  width: 1px;
  height: 100%;
  transform-origin: 100% 50%;
  transform: scaleX(calc(1 / var(--f7-device-pixel-ratio)));
}
.timeline-year:last-child:after {
  display: none !important;
}
.timeline-month {
  padding-top: var(--f7-timeline-month-height);
}
.timeline-month .timeline-item:before {
  content: '';
  position: absolute;
  background-color: var(--f7-timeline-horizontal-item-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.timeline-year,
.timeline-month {
  display: flex;
  flex-shrink: 0;
  position: relative;
  box-sizing: border-box;
  height: 100%;
}
.timeline-year-title {
  line-height: var(--f7-timeline-year-height);
  height: var(--f7-timeline-year-height);
  font-size: var(--f7-timeline-year-font-size);
  font-weight: var(--f7-timeline-year-font-weight);
}
.timeline-month-title {
  line-height: var(--f7-timeline-month-height);
  height: var(--f7-timeline-month-height);
  font-size: var(--f7-timeline-month-font-size);
  font-weight: var(--f7-timeline-month-font-weight);
}
.timeline-year-title,
.timeline-month-title {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  box-sizing: border-box;
  padding: 0 var(--f7-timeline-horizontal-item-padding);
  background-color: var(--f7-bars-bg-color);
  color: var(--f7-bars-text-color);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .timeline-year-title,
  .ios-translucent-bars .timeline-month-title {
    background-color: rgba(var(--f7-bars-bg-color-rgb), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.timeline-year-title span,
.timeline-month-title span {
  display: inline-block;
  position: -webkit-sticky;
  position: sticky;
  left: calc(var(--f7-timeline-horizontal-item-padding) + var(--f7-safe-area-left));
}
.timeline-month-title span {
  margin-top: -2px;
}
.timeline-year:first-child .timeline-year-title,
.timeline-year:first-child .timeline-month:first-child .timeline-month-title,
.timeline-year:first-child .timeline-year-title + .timeline-month .timeline-month-title {
  left: calc(var(--f7-safe-area-left) * -1);
  right: 0;
  width: auto;
}
.timeline-horizontal .timeline-item:first-child,
.timeline-year:first-child .timeline-month:first-child .timeline-item:first-child,
.timeline-year:first-child .timeline-year-title + .timeline-month .timeline-item:first-child,
.timeline-year:first-child .timeline-year-title + .timeline-month .timeline-month-title + .timeline-item {
  overflow: visible;
}
.timeline-horizontal .timeline-item:first-child .timeline-item-date,
.timeline-year:first-child .timeline-month:first-child .timeline-item:first-child .timeline-item-date,
.timeline-year:first-child .timeline-year-title + .timeline-month .timeline-item:first-child .timeline-item-date,
.timeline-year:first-child .timeline-year-title + .timeline-month .timeline-month-title + .timeline-item .timeline-item-date {
  width: auto;
  padding-left: calc(var(--f7-timeline-horizontal-item-padding) + var(--f7-safe-area-left));
  left: calc(0px - var(--f7-safe-area-left));
  right: 0;
}
.timeline-year:last-child .timeline-year-title,
.timeline-year:last-child .timeline-month:last-child .timeline-month-title {
  width: auto;
  right: calc(0px - var(--f7-safe-area-right));
}
.timeline-horizontal .timeline-item:last-child,
.timeline-year:last-child .timeline-month:last-child .timeline-item:last-child {
  overflow: visible;
}
.timeline-horizontal .timeline-item:last-child .timeline-item-date,
.timeline-year:last-child .timeline-month:last-child .timeline-item:last-child .timeline-item-date {
  width: auto;
  right: calc(0px - var(--f7-safe-area-right));
  left: 0;
}
.ios .block-strong .timeline-item-inner {
  border-radius: 3px;
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.ios .timeline-year-title span {
  margin-top: 3px;
}
.md .timeline-year-title span {
  margin-top: 2px;
}
.aurora .timeline-year-title span {
  margin-top: 2px;
}
/* === Tabs === */
.tabs .tab {
  display: none;
}
.tabs .tab-active {
  display: block;
}
.tabs-animated-wrap {
  position: relative;
  width: 100%;
  overflow: hidden;
  height: 100%;
}
.tabs-animated-wrap > .tabs {
  display: flex;
  height: 100%;
  transition-duration: 300ms;
}
.tabs-animated-wrap > .tabs > .tab {
  width: 100%;
  display: block;
  flex-shrink: 0;
}
.tabs-animated-wrap.not-animated > .tabs {
  transition-duration: 0ms;
}
.tabs-swipeable-wrap {
  height: 100%;
}
.tabs-swipeable-wrap > .tabs {
  height: 100%;
}
.tabs-swipeable-wrap > .tabs > .tab {
  display: block;
}
.page > .tabs {
  height: 100%;
}
/* === Panels === */
:root {
  --f7-panel-width: 260px;
  /*
  --f7-panel-left-width: var(--f7-panel-width);
  --f7-panel-right-width: var(--f7-panel-width);
  --f7-panel-left-collapsed-width: var(--f7-panel-collapsed-width);
  --f7-panel-right-collapsed-width: var(--f7-panel-collapsed-width);
  */
  --f7-panel-bg-color: #fff;
}
.ios {
  --f7-panel-collapsed-width: 58px;
  --f7-panel-backdrop-bg-color: rgba(0, 0, 0, 0);
  --f7-panel-transition-duration: 400ms;
  --f7-panel-shadow: transparent;
}
.md {
  --f7-panel-collapsed-width: 60px;
  --f7-panel-backdrop-bg-color: rgba(0, 0, 0, 0.3);
  --f7-panel-transition-duration: 300ms;
  --f7-panel-shadow: rgba(0, 0, 0, 0.2) 0%,
    rgba(0, 0, 0, 0.07) 30%,
    rgba(0, 0, 0, 0.03) 40%,
    rgba(0, 0, 0, 0) 60%,
    rgba(0, 0, 0, 0) 100%;
}
.aurora {
  --f7-panel-collapsed-width: 44px;
  --f7-panel-backdrop-bg-color: rgba(0, 0, 0, 0.2);
  --f7-panel-transition-duration: 400ms;
  --f7-panel-shadow: transparent;
}
.panel-backdrop {
  position: absolute;
  left: 0;
  top: var(--f7-appbar-app-offset, 0px);
  width: 100%;
  height: calc(100% - var(--f7-appbar-app-offset, 0px));
  opacity: 0;
  z-index: 5999;
  visibility: hidden;
  pointer-events: none;
  transform: translate3d(0, 0, 0);
  background-color: var(--f7-panel-backdrop-bg-color);
  transition-property: transform, opacity;
  transition-duration: var(--f7-panel-transition-duration);
}
.panel-backdrop .with-panel,
.panel-backdrop .with-panel-closing {
  visibility: visible;
}
.panel-backdrop.not-animated {
  transition-duration: 0ms !important;
}
.panel {
  z-index: 1000;
  box-sizing: border-box;
  position: absolute;
  top: var(--f7-appbar-app-offset, 0px);
  height: calc(100% - var(--f7-appbar-app-offset, 0px));
  transform: translate3d(0, 0, 0);
  width: var(--f7-panel-width);
  background-color: var(--f7-panel-bg-color);
  overflow: visible;
  transition-property: transform;
  transition-duration: var(--f7-panel-transition-duration);
}
.panel:not(.panel-in):not(.panel-out):not(.panel-in-breakpoint):not(.panel-in-collapsed):not(.panel-in-swipe) {
  display: none;
}
.panel:after {
  pointer-events: none;
  opacity: 0;
  z-index: 5999;
  position: absolute;
  content: '';
  top: 0;
  width: 20px;
  height: 100%;
  transition-property: transform, opacity;
  transition-duration: var(--f7-panel-transition-duration);
}
.panel.not-animated,
.panel.not-animated:after {
  transition-duration: 0ms !important;
}
.panel.panel-reveal.not-animated ~ .views,
.panel.panel-reveal.not-animated ~ .view {
  transition-duration: 0ms !important;
}
.panel.panel-resizing {
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
}
.panel.panel-resizing,
.panel.panel-resizing:after,
.panel.panel-resizing ~ .views,
.panel.panel-resizing ~ .view {
  transition-duration: 0ms !important;
}
.panel-cover {
  z-index: 6000;
}
.panel-left {
  left: 0;
  width: var(--f7-panel-left-width, var(--f7-panel-width));
}
.panel-left.panel-cover {
  transform: translate3d(-100%, 0, 0);
}
.panel-left.panel-cover:after {
  left: 100%;
  background: linear-gradient(to right, var(--f7-panel-shadow));
}
html.with-panel-left-cover .panel-left.panel-cover:after {
  opacity: 1;
}
.panel-left.panel-reveal:after {
  right: 0;
  transform: translate3d(calc(-1 * var(--f7-panel-left-width, var(--f7-panel-width))), 0, 0);
  background: linear-gradient(to left, var(--f7-panel-shadow));
}
html.with-panel-left-reveal .panel-left.panel-reveal:after {
  opacity: 1;
  transform: translate3d(0, 0, 0);
}
.panel-right {
  right: 0;
  width: var(--f7-panel-right-width, var(--f7-panel-width));
}
.panel-right.panel-cover {
  transform: translate3d(100%, 0, 0);
}
.panel-right.panel-cover:after {
  right: 100%;
  background: linear-gradient(to left, var(--f7-panel-shadow));
}
html.with-panel-right-cover .panel-right.panel-cover:after {
  opacity: 1;
}
.panel-right.panel-reveal:after {
  left: 0;
  background: linear-gradient(to right, var(--f7-panel-shadow));
  transform: translate3d(var(--f7-panel-right-width, var(--f7-panel-width)), 0, 0);
}
html.with-panel-right-reveal .panel-right.panel-reveal:after {
  opacity: 1;
  transform: translate3d(0, 0, 0);
}
.panel-in-breakpoint {
  transform: translate3d(0, 0, 0) !important;
  transition-duration: 0ms;
}
.panel-in-breakpoint:after {
  display: none;
}
.panel-in-breakpoint.panel-cover {
  z-index: 5900;
}
html.with-panel-left-reveal .views,
html.with-panel-right-reveal .views,
html.with-panel-closing .views,
html.with-panel-left-reveal .framework7-root > .view,
html.with-panel-right-reveal .framework7-root > .view,
html.with-panel-closing .framework7-root > .view {
  transition-duration: var(--f7-panel-transition-duration);
  transition-property: transform;
}
html.with-panel-left-reveal .panel-backdrop,
html.with-panel-right-reveal .panel-backdrop,
html.with-panel-closing .panel-backdrop {
  visibility: visible;
  pointer-events: auto;
  opacity: 0;
}
html.with-panel .framework7-root > .views .page-content,
html.with-panel .framework7-root > .view .page-content {
  overflow: hidden;
  -webkit-overflow-scrolling: auto;
}
html.with-panel-left-cover .panel-backdrop,
html.with-panel-right-cover .panel-backdrop {
  visibility: visible;
  pointer-events: auto;
  opacity: 1;
}
html.with-panel-left-reveal .views,
html.with-panel-left-reveal .framework7-root > .view,
html.with-panel-left-reveal .panel-backdrop {
  transform: translate3d(var(--f7-panel-left-width, var(--f7-panel-width)), 0, 0);
}
html.with-panel-right-reveal .views,
html.with-panel-right-reveal .framework7-root > .view,
html.with-panel-right-reveal .panel-backdrop {
  transform: translate3d(calc(-1 * var(--f7-panel-right-width, var(--f7-panel-width))), 0, 0);
}
html.with-panel-left-cover .panel-left {
  transform: translate3d(0px, 0, 0);
}
html.with-panel-right-cover .panel-right {
  transform: translate3d(0px, 0, 0);
}
.panel-resize-handler {
  position: absolute;
  top: 0;
  height: 100%;
  width: 6px;
  cursor: col-resize;
  z-index: 6000;
  display: none;
}
.panel-resizable .panel-resize-handler {
  display: block;
}
.panel-left.panel-cover .panel-resize-handler {
  right: -3px;
}
.panel-left.panel-reveal .panel-resize-handler {
  right: 0;
}
.panel-right.panel-cover .panel-resize-handler {
  left: -3px;
}
.panel-right.panel-reveal .panel-resize-handler {
  left: 0;
}
.panel-left.panel-in-collapsed ~ .views,
.panel-left.panel-in-collapsed ~ .view {
  margin-left: var(--f7-panel-left-collapsed-width, var(--f7-panel-collapsed-width));
}
html.with-panel-left-reveal .panel-left.panel-in-collapsed ~ .views,
html.with-panel-left-reveal .panel-left.panel-in-collapsed ~ .view {
  transform: translate3d(calc(var(--f7-panel-left-width, var(--f7-panel-width)) - var(--f7-panel-left-collapsed-width, var(--f7-panel-collapsed-width))), 0, 0);
}
.panel-right.panel-in-collapsed ~ .views,
.panel-right.panel-in-collapsed ~ .view {
  margin-right: var(--f7-panel-right-collapsed-width, var(--f7-panel-collapsed-width));
}
html.with-panel-right-reveal .panel-right.panel-in-collapsed ~ .views,
html.with-panel-right-reveal .panel-right.panel-in-collapsed ~ .view {
  transform: translate3d(calc(var(--f7-panel-right-collapsed-width, var(--f7-panel-collapsed-width)) - var(--f7-panel-right-width, var(--f7-panel-width))), 0, 0);
}
/* === Card === */
:root {
  --f7-card-content-padding-horizontal: 16px;
  --f7-card-content-padding-vertical: 16px;
  --f7-card-border-radius: 4px;
  --f7-card-font-size: inherit;
  --f7-card-header-text-color: inherit;
  --f7-card-header-font-weight: 400;
  --f7-card-header-padding-horizontal: 16px;
  --f7-card-footer-font-weight: 400;
  --f7-card-footer-font-size: inherit;
  --f7-card-footer-padding-horizontal: 16px;
  --f7-card-expandable-font-size: 16px;
  --f7-card-expandable-tablet-width: 670px;
  --f7-card-expandable-tablet-height: 670px;
  --f7-card-bg-color: #fff;
  --f7-card-outline-border-color: rgba(0, 0, 0, 0.12);
  --f7-card-header-border-color: rgba(0, 0, 0, 0.1);
  --f7-card-footer-border-color: rgba(0, 0, 0, 0.1);
  --f7-card-expandable-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-card-bg-color: #1c1c1d;
  --f7-card-expandable-bg-color: #1c1c1d;
  --f7-card-outline-border-color: rgba(255, 255, 255, 0.15);
  --f7-card-header-border-color: rgba(255, 255, 255, 0.15);
  --f7-card-footer-border-color: rgba(255, 255, 255, 0.15);
  --f7-card-footer-text-color: rgba(255, 255, 255, 0.55);
}
.ios {
  --f7-card-margin-horizontal: 10px;
  --f7-card-margin-vertical: 10px;
  --f7-card-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.2);
  --f7-card-header-font-size: 17px;
  --f7-card-header-padding-vertical: 10px;
  --f7-card-header-min-height: 44px;
  --f7-card-footer-text-color: rgba(0, 0, 0, 0.45);
  --f7-card-footer-padding-vertical: 10px;
  --f7-card-footer-min-height: 44px;
  --f7-card-expandable-margin-horizontal: 20px;
  --f7-card-expandable-margin-vertical: 30px;
  --f7-card-expandable-box-shadow: 0px 20px 40px rgba(0, 0, 0, 0.3);
  --f7-card-expandable-border-radius: 15px;
  --f7-card-expandable-tablet-border-radius: 5px;
  --f7-card-expandable-header-font-size: 27px;
  --f7-card-expandable-header-font-weight: bold;
}
.md {
  --f7-card-margin-horizontal: 8px;
  --f7-card-margin-vertical: 8px;
  --f7-card-box-shadow: var(--f7-elevation-1);
  --f7-card-header-font-size: 16px;
  --f7-card-header-padding-vertical: 4px;
  --f7-card-header-min-height: 48px;
  --f7-card-footer-text-color: rgba(0, 0, 0, 0.54);
  --f7-card-footer-padding-vertical: 4px;
  --f7-card-footer-min-height: 48px;
  --f7-card-expandable-margin-horizontal: 12px;
  --f7-card-expandable-margin-vertical: 24px;
  --f7-card-expandable-box-shadow: var(--f7-elevation-10);
  --f7-card-expandable-border-radius: 8px;
  --f7-card-expandable-tablet-border-radius: 4px;
  --f7-card-expandable-header-font-size: 24px;
  --f7-card-expandable-header-font-weight: 500;
}
.aurora {
  --f7-card-margin-horizontal: 10px;
  --f7-card-margin-vertical: 10px;
  --f7-card-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.15);
  --f7-card-header-font-size: 14px;
  --f7-card-header-font-weight: bold;
  --f7-card-header-padding-vertical: 10px;
  --f7-card-header-min-height: 38px;
  --f7-card-footer-text-color: rgba(0, 0, 0, 0.6);
  --f7-card-footer-padding-vertical: 10px;
  --f7-card-footer-min-height: 38px;
  --f7-card-expandable-margin-horizontal: 10px;
  --f7-card-expandable-margin-vertical: 20px;
  --f7-card-expandable-box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.15);
  --f7-card-expandable-border-radius: 15px;
  --f7-card-expandable-tablet-border-radius: 5px;
  --f7-card-expandable-header-font-size: 27px;
  --f7-card-expandable-header-font-weight: bold;
}
.cards-list > ul:before,
.card .list > ul:before,
.cards-list > ul:after,
.card .list > ul:after {
  display: none !important;
}
.cards-list ul,
.card .list ul {
  background: none;
}
.card {
  background: var(--f7-card-bg-color);
  position: relative;
  border-radius: var(--f7-card-border-radius);
  font-size: var(--f7-card-font-size);
  margin-top: var(--f7-card-margin-vertical);
  margin-bottom: var(--f7-card-margin-vertical);
  margin-left: calc(var(--f7-card-margin-horizontal) + var(--f7-safe-area-left));
  margin-right: calc(var(--f7-card-margin-horizontal) + var(--f7-safe-area-right));
  box-shadow: var(--f7-card-box-shadow);
}
.card .list,
.card .block {
  margin: 0;
}
.row:not(.no-gap) .col > .card {
  margin-left: 0;
  margin-right: 0;
}
.card.no-shadow {
  box-shadow: none;
}
.card-outline,
.ios .card-outline-ios,
.md .card-outline-md,
.aurora .card-outline-aurora {
  box-shadow: none;
  border: 1px solid var(--f7-card-outline-border-color);
}
.card-outline.no-border,
.ios .card-outline-ios.no-border,
.md .card-outline-md.no-border,
.aurora .card-outline-aurora.no-border,
.card-outline.no-hairlines,
.ios .card-outline-ios.no-hairlines,
.md .card-outline-md.no-hairlines,
.aurora .card-outline-aurora.no-hairlines {
  border: none;
}
.card-content {
  position: relative;
}
.card-content-padding {
  position: relative;
  padding: var(--f7-card-content-padding-vertical) var(--f7-card-content-padding-horizontal);
}
.card-content-padding > .list,
.card-content-padding > .block {
  margin: calc(-1 * var(--f7-card-content-padding-vertical)) calc(-1 * var(--f7-card-content-padding-horizontal));
}
.card-content-padding > p:first-child {
  margin-top: 0;
}
.card-content-padding > p:last-child {
  margin-bottom: 0;
}
.card-header {
  min-height: var(--f7-card-header-min-height);
  color: var(--f7-card-header-text-color);
  font-size: var(--f7-card-header-font-size);
  font-weight: var(--f7-card-header-font-weight);
  padding: var(--f7-card-header-padding-vertical) var(--f7-card-header-padding-horizontal);
}
.card-footer {
  min-height: var(--f7-card-footer-min-height);
  color: var(--f7-card-footer-text-color);
  font-size: var(--f7-card-footer-font-size);
  font-weight: var(--f7-card-footer-font-weight);
  padding: var(--f7-card-footer-padding-vertical) var(--f7-card-footer-padding-horizontal);
}
.card-footer a.link {
  overflow: hidden;
}
.card-header,
.card-footer {
  position: relative;
  box-sizing: border-box;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.card-header[valign="top"],
.card-footer[valign="top"] {
  align-items: flex-start;
}
.card-header[valign="bottom"],
.card-footer[valign="bottom"] {
  align-items: flex-end;
}
.card-header a.link,
.card-footer a.link {
  position: relative;
}
.card-header a.link i.icon,
.card-footer a.link i.icon {
  display: block;
}
.card-header a.icon-only,
.card-footer a.icon-only {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
}
.card-header {
  border-radius: var(--f7-card-border-radius) var(--f7-card-border-radius) 0 0;
}
.card-header:after {
  content: '';
  position: absolute;
  background-color: var(--f7-card-header-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.card-header.no-hairline:after {
  display: none !important;
}
.card-footer {
  border-radius: 0 0 var(--f7-card-border-radius) var(--f7-card-border-radius);
}
.card-footer:before {
  content: '';
  position: absolute;
  background-color: var(--f7-card-footer-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.card-footer.no-hairline:before {
  display: none !important;
}
.card-expandable {
  overflow: hidden;
  height: 300px;
  background: var(--f7-card-expandable-bg-color);
  position: relative;
  transform-origin: center center;
  transition-property: transform, border-radius;
  border-radius: var(--f7-card-expandable-border-radius);
  z-index: 2;
  transition-duration: 200ms;
  margin-left: calc(var(--f7-card-expandable-margin-horizontal) + var(--f7-safe-area-left));
  margin-right: calc(var(--f7-card-expandable-margin-horizontal) + var(--f7-safe-area-right));
  margin-top: var(--f7-card-expandable-margin-vertical);
  margin-bottom: var(--f7-card-expandable-margin-vertical);
  box-shadow: var(--f7-card-expandable-box-shadow);
  font-size: var(--f7-card-expandable-font-size);
}
.card-expandable.card-no-transition {
  transition-duration: 0ms;
}
.card-expandable.card-expandable-animate-width .card-content {
  transition-property: width, transform;
  width: 100%;
}
.card-expandable.active-state {
  transform: scale(0.97);
}
.card-expandable .card-opened-fade-in,
.card-expandable .card-opened-fade-out {
  transition-duration: 400ms;
}
.card-expandable .card-opened-fade-in {
  opacity: 0;
  pointer-events: none;
}
.card-expandable .card-content {
  position: absolute;
  top: 0;
  width: 100vw;
  height: 100vh;
  transform-origin: center top;
  overflow: hidden;
  transition-property: transform;
  box-sizing: border-box;
  pointer-events: none;
  left: 0;
}
.card-expandable .card-content .card-content-padding {
  padding-left: calc(var(--f7-safe-area-left) + var(--f7-card-content-padding-horizontal));
  padding-right: calc(var(--f7-safe-area-right) + var(--f7-card-content-padding-horizontal));
}
.card-expandable.card-opened {
  transition-duration: 0ms;
}
.card-expandable.card-opening,
.card-expandable.card-closing,
.card-expandable.card-transitioning {
  transition-duration: 400ms;
}
.card-expandable.card-opening .card-content {
  transition-duration: 300ms;
}
.card-expandable.card-closing .card-content {
  transition-duration: 500ms;
}
.card-expandable.card-opening,
.card-expandable.card-opened,
.card-expandable.card-closing {
  z-index: 100;
}
.card-expandable.card-opening,
.card-expandable.card-opened {
  border-radius: 0;
}
.card-expandable.card-opening .card-opened-fade-in,
.card-expandable.card-opened .card-opened-fade-in {
  opacity: 1;
  pointer-events: auto;
}
.card-expandable.card-opening .card-opened-fade-out,
.card-expandable.card-opened .card-opened-fade-out {
  opacity: 0;
  pointer-events: none;
}
.card-expandable.card-opened .card-content {
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  pointer-events: auto;
}
.card-expandable .card-header {
  font-size: var(--f7-card-expandable-header-font-size);
  font-weight: var(--f7-card-expandable-header-font-weight);
}
.card-expandable .card-header:after {
  display: none !important;
}
.card-prevent-open {
  pointer-events: auto;
}
.card-expandable-size {
  width: 0;
  height: 0;
  position: absolute;
  left: 0;
  top: 0;
  opacity: 0;
  pointer-events: none;
  visibility: hidden;
}
@media (min-width: 768px) and (min-height: 670px) {
  .card-expandable:not(.card-tablet-fullscreen) {
    max-width: var(--f7-card-expandable-tablet-width);
  }
  .card-expandable:not(.card-tablet-fullscreen).card-opened,
  .card-expandable:not(.card-tablet-fullscreen).card-opening {
    border-radius: var(--f7-card-expandable-tablet-border-radius);
  }
  .card-expandable:not(.card-tablet-fullscreen):not(.card-expandable-animate-width) .card-content {
    width: var(--f7-card-expandable-tablet-width);
  }
  .card-expandable:not(.card-tablet-fullscreen) .card-expandable-size {
    width: var(--f7-card-expandable-tablet-width);
    height: var(--f7-card-expandable-tablet-height);
  }
}
.page.page-with-card-opened .page-content {
  overflow: hidden;
}
.card-backdrop {
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: 99;
  pointer-events: none;
  background: rgba(0, 0, 0, 0.2);
  opacity: 0;
}
.card-backdrop-in {
  animation: card-backdrop-fade-in 400ms forwards;
  pointer-events: auto;
}
.card-backdrop-out {
  animation: card-backdrop-fade-out 400ms forwards;
}
@supports ((-webkit-backdrop-filter: blur(15px)) or (backdrop-filter: blur(15px))) {
  .card-backdrop {
    background: transparent;
    opacity: 1;
  }
  .card-backdrop-in {
    animation: card-backdrop-blur-in 400ms forwards;
  }
  .card-backdrop-out {
    animation: card-backdrop-blur-out 400ms forwards;
  }
}
@keyframes card-backdrop-fade-in {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes card-backdrop-fade-out {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@keyframes card-backdrop-blur-in {
  from {
    -webkit-backdrop-filter: blur(0px);
            backdrop-filter: blur(0px);
  }
  to {
    -webkit-backdrop-filter: blur(15px);
            backdrop-filter: blur(15px);
  }
}
@keyframes card-backdrop-blur-out {
  from {
    -webkit-backdrop-filter: blur(15px);
            backdrop-filter: blur(15px);
  }
  to {
    -webkit-backdrop-filter: blur(0px);
            backdrop-filter: blur(0px);
  }
}
/* === Chips === */
:root {
  --f7-chip-font-size: 13px;
  --f7-chip-font-weight: normal;
  --f7-chip-media-font-size: 16px;
  --f7-chip-bg-color: rgba(0, 0, 0, 0.12);
  --f7-chip-outline-border-color: rgba(0, 0, 0, 0.12);
  --f7-chip-delete-button-color: #000;
}
:root .theme-dark,
:root.theme-dark {
  --f7-chip-delete-button-color: #fff;
  --f7-chip-bg-color: #333;
  --f7-chip-outline-border-color: rgba(255, 255, 255, 0.12);
}
.ios {
  --f7-chip-height: 24px;
  --f7-chip-padding-horizontal: 10px;
  --f7-chip-text-color: #000;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-chip-text-color: #fff;
}
.md {
  --f7-chip-height: 32px;
  --f7-chip-padding-horizontal: 12px;
  --f7-chip-text-color: rgba(0, 0, 0, 0.87);
}
.md .theme-dark,
.md.theme-dark {
  --f7-chip-text-color: rgba(255, 255, 255, 0.87);
}
.aurora {
  --f7-chip-height: 20px;
  --f7-chip-padding-horizontal: 10px;
  --f7-chip-font-size: 12px;
  --f7-chip-media-font-size: 14px;
  --f7-chip-text-color: #000;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-chip-text-color: #fff;
}
.chip {
  padding-left: var(--f7-chip-padding-horizontal);
  padding-right: var(--f7-chip-padding-horizontal);
  font-weight: var(--f7-chip-font-weight);
  display: inline-flex;
  box-sizing: border-box;
  vertical-align: middle;
  align-items: center;
  margin: 2px 0;
  background-color: var(--f7-chip-bg-color);
  font-size: var(--f7-chip-font-size);
  color: var(--f7-chip-text-color);
  height: var(--f7-chip-height);
  line-height: var(--f7-chip-height);
  border-radius: var(--f7-chip-height);
  position: relative;
}
.chip-media {
  border-radius: 50%;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  height: var(--f7-chip-height);
  width: var(--f7-chip-height);
  border-radius: var(--f7-chip-height);
  text-align: center;
  line-height: var(--f7-chip-height);
  box-sizing: border-box;
  color: #fff;
  font-size: var(--f7-chip-media-font-size);
  vertical-align: middle;
  margin-left: calc(-1 * var(--f7-chip-padding-horizontal));
}
.chip-media i.icon {
  font-size: calc(var(--f7-chip-height) - 8px);
  height: calc(var(--f7-chip-height) - 8px);
}
.chip-media img {
  max-width: 100%;
  max-height: 100%;
  width: auto;
  height: auto;
  border-radius: 50%;
  display: block;
}
.chip-media + .chip-label {
  margin-left: 4px;
}
.chip-label {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  position: relative;
  flex-shrink: 1;
  min-width: 0;
}
.chip-delete {
  text-align: center;
  cursor: pointer;
  flex-shrink: 0;
  background-repeat: no-repeat;
  width: 24px;
  height: 24px;
  color: var(--f7-chip-delete-button-color);
  opacity: 0.54;
  position: relative;
}
.chip-delete:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  content: 'delete_round_ios';
  line-height: 24px;
}
.chip .chip-delete.active-state {
  opacity: 1;
}
.chip-outline,
.ios .chip-outline-ios,
.md .chip-outline-md,
.aurora .chip-outline-aurora {
  border: 1px solid var(--f7-chip-outline-border-color);
  background: none;
}
.chip[class*="color-"] {
  --f7-chip-bg-color: var(--f7-theme-color);
  --f7-chip-text-color: #fff;
}
.chip-outline[class*="color-"],
.ios .chip-outline-ios[class*="color-"],
.md .chip-outline-md[class*="color-"],
.aurora .chip-outline-aurora[class*="color-"] {
  --f7-chip-outline-border-color: var(--f7-theme-color);
  --f7-chip-text-color: var(--f7-theme-color);
}
.ios .chip-delete {
  margin-right: calc(-1 * var(--f7-chip-padding-horizontal));
}
.ios .chip-delete:after {
  font-size: 10px;
}
.md .chip-label + .chip-delete {
  margin-left: 4px;
}
.md .chip-delete {
  margin-right: calc(-1 * var(--f7-chip-padding-horizontal) + 4px);
}
.md .chip-delete:after {
  font-size: 12px;
}
.aurora .chip-delete {
  margin-right: calc(-1 * var(--f7-chip-padding-horizontal));
}
.aurora .chip-delete:after {
  font-size: 10px;
}
/* === Form === */
/* === Input === */
:root {
  --f7-input-bg-color: transparent;
  --f7-label-font-weight: 400;
  --f7-label-line-height: 1.2;
  --f7-input-padding-left: 0px;
  --f7-input-padding-right: 0px;
  --f7-input-error-text-color: #ff3b30;
  --f7-input-error-font-size: 12px;
  --f7-input-error-line-height: 1.4;
  --f7-input-error-font-weight: 400;
  --f7-input-info-font-size: 12px;
  --f7-input-info-line-height: 1.4;
  --f7-input-outline-height: 40px;
  --f7-input-outline-border-radius: 4px;
  --f7-input-outline-padding-horizontal: 12px;
  --f7-textarea-height: 100px;
  /*
  --f7-input-outline-focused-border-color: var(--f7-theme-color);
  --f7-input-outline-invalid-border-color: var(--f7-input-error-text-color);
  */
  --f7-input-outline-border-color: #999;
}
:root .theme-dark,
:root.theme-dark {
  --f7-input-outline-border-color: #444;
}
.ios {
  --f7-input-height: 44px;
  --f7-input-font-size: 17px;
  --f7-input-placeholder-color: #a9a9a9;
  --f7-textarea-padding-vertical: 11px;
  /*
  --f7-input-focused-border-color: var(--f7-list-item-border-color);
  --f7-input-invalid-border-color: var(--f7-list-item-border-color);
  --f7-input-invalid-text-color: var(--f7-input-error-text-color);
  */
  --f7-label-font-size: 12px;
  --f7-label-text-color: inherit;
  /*
  --f7-label-focused-text-color: var(--f7-label-text-color);
  --f7-label-invalid-text-color: var(--f7-label-text-color);
  */
  --f7-floating-label-scale: calc(17 / 12);
  --f7-inline-label-font-size: 17px;
  --f7-inline-label-line-height: 1.4;
  --f7-inline-label-padding-top: 3px;
  --f7-input-clear-button-size: 14px;
  --f7-input-text-color: #000000;
  --f7-input-info-text-color: rgba(0, 0, 0, 0.45);
  --f7-input-clear-button-color: rgba(0, 0, 0, 0.45);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-input-text-color: #fff;
  --f7-input-info-text-color: rgba(255, 255, 255, 0.55);
  --f7-input-clear-button-color: rgba(255, 255, 255, 0.5);
}
.md {
  --f7-input-height: 36px;
  --f7-input-font-size: 16px;
  --f7-textarea-padding-vertical: 7px;
  /*
  --f7-input-focused-border-color: var(--f7-theme-color);
  --f7-input-invalid-border-color: var(--f7-input-error-text-color);
  --f7-input-invalid-text-color: var(--f7-input-text-color);
  */
  --f7-label-font-size: 12px;
  /*
  --f7-label-focused-text-color: var(--f7-theme-color);
  --f7-label-invalid-text-color: var(--f7-input-error-text-color );
  */
  --f7-floating-label-scale: calc(16 / 12);
  --f7-inline-label-font-size: 16px;
  --f7-inline-label-line-height: 1.5;
  --f7-inline-label-padding-top: 7px;
  --f7-input-clear-button-size: 18px;
  --f7-input-clear-button-color: #aaa;
  --f7-input-text-color: #212121;
  --f7-input-placeholder-color: rgba(0, 0, 0, 0.35);
  --f7-label-text-color: rgba(0, 0, 0, 0.65);
  --f7-input-info-text-color: rgba(0, 0, 0, 0.45);
}
.md .theme-dark,
.md.theme-dark {
  --f7-input-text-color: rgba(255, 255, 255, 0.87);
  --f7-input-placeholder-color: rgba(255, 255, 255, 0.35);
  --f7-label-text-color: rgba(255, 255, 255, 0.54);
  --f7-input-info-text-color: rgba(255, 255, 255, 0.45);
}
.aurora {
  --f7-input-height: 24px;
  --f7-input-font-size: 13px;
  --f7-textarea-padding-vertical: 2px;
  /*
  --f7-input-focused-border-color: var(--f7-list-item-border-color);
  --f7-input-invalid-border-color: var(--f7-list-item-border-color);
  --f7-input-invalid-text-color: var(--f7-input-error-text-color);
  */
  --f7-label-font-size: 11px;
  --f7-label-text-color: inherit;
  /*
  --f7-label-focused-text-color: var(--f7-label-text-color);
  --f7-label-invalid-text-color: var(--f7-label-text-color);
  */
  --f7-floating-label-scale: calc(13 / 11);
  --f7-inline-label-font-size: 14px;
  --f7-inline-label-line-height: 1.4;
  --f7-inline-label-padding-top: 1px;
  --f7-input-clear-button-size: 14px;
  --f7-input-outline-height: 32px;
  --f7-input-outline-padding-horizontal: 8px;
  --f7-input-text-color: #000000;
  --f7-input-placeholder-color: rgba(0, 0, 0, 0.32);
  --f7-input-clear-button-color: #666;
  --f7-input-info-text-color: rgba(0, 0, 0, 0.5);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-input-text-color: #fff;
  --f7-input-clear-button-color: #aaa;
  --f7-input-placeholder-color: rgba(255, 255, 255, 0.35);
  --f7-input-info-text-color: rgba(255, 255, 255, 0.45);
}
input[type="text"],
input[type="password"],
input[type="search"],
input[type="email"],
input[type="tel"],
input[type="url"],
input[type="date"],
input[type="datetime-local"],
input[type="time"],
input[type="number"],
select,
textarea {
  box-sizing: border-box;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  border: none;
  box-shadow: none;
  border-radius: 0;
  outline: 0;
  display: block;
  padding: 0;
  margin: 0;
  font-family: inherit;
  background: none;
  resize: none;
  font-size: inherit;
  color: inherit;
}
.textarea-resizable-shadow {
  opacity: 0;
  position: absolute;
  z-index: -1000;
  pointer-events: none;
  left: -1000px;
  top: -1000px;
  visibility: hidden;
}
.list input[type="text"],
.list input[type="password"],
.list input[type="search"],
.list input[type="email"],
.list input[type="tel"],
.list input[type="url"],
.list input[type="date"],
.list input[type="datetime-local"],
.list input[type="time"],
.list input[type="number"],
.list select {
  width: 100%;
  height: var(--f7-input-height);
  color: var(--f7-input-text-color);
  font-size: var(--f7-input-font-size);
  background-color: var(--f7-input-bg-color, transparent);
  padding-left: var(--f7-input-padding-left);
  padding-right: var(--f7-input-padding-right);
}
.list input[type="text"]::-webkit-input-placeholder,
.list input[type="password"]::-webkit-input-placeholder,
.list input[type="search"]::-webkit-input-placeholder,
.list input[type="email"]::-webkit-input-placeholder,
.list input[type="tel"]::-webkit-input-placeholder,
.list input[type="url"]::-webkit-input-placeholder,
.list input[type="date"]::-webkit-input-placeholder,
.list input[type="datetime-local"]::-webkit-input-placeholder,
.list input[type="time"]::-webkit-input-placeholder,
.list input[type="number"]::-webkit-input-placeholder,
.list select::-webkit-input-placeholder {
  color: var(--f7-input-placeholder-color);
}
.list input[type="text"]::-moz-placeholder,
.list input[type="password"]::-moz-placeholder,
.list input[type="search"]::-moz-placeholder,
.list input[type="email"]::-moz-placeholder,
.list input[type="tel"]::-moz-placeholder,
.list input[type="url"]::-moz-placeholder,
.list input[type="date"]::-moz-placeholder,
.list input[type="datetime-local"]::-moz-placeholder,
.list input[type="time"]::-moz-placeholder,
.list input[type="number"]::-moz-placeholder,
.list select::-moz-placeholder {
  color: var(--f7-input-placeholder-color);
}
.list input[type="text"]::placeholder,
.list input[type="password"]::placeholder,
.list input[type="search"]::placeholder,
.list input[type="email"]::placeholder,
.list input[type="tel"]::placeholder,
.list input[type="url"]::placeholder,
.list input[type="date"]::placeholder,
.list input[type="datetime-local"]::placeholder,
.list input[type="time"]::placeholder,
.list input[type="number"]::placeholder,
.list select::placeholder {
  color: var(--f7-input-placeholder-color);
}
.list textarea {
  width: 100%;
  color: var(--f7-input-text-color);
  font-size: var(--f7-input-font-size);
  resize: none;
  line-height: 1.4;
  height: var(--f7-textarea-height);
  background-color: var(--f7-input-bg-color, transparent);
  padding-top: var(--f7-textarea-padding-vertical);
  padding-bottom: var(--f7-textarea-padding-vertical);
  padding-left: var(--f7-input-padding-left);
  padding-right: var(--f7-input-padding-right);
}
.list textarea::-webkit-input-placeholder {
  color: var(--f7-input-placeholder-color);
}
.list textarea::-moz-placeholder {
  color: var(--f7-input-placeholder-color);
}
.list textarea::placeholder {
  color: var(--f7-input-placeholder-color);
}
.list textarea.resizable {
  height: var(--f7-input-height);
}
.list input[type="datetime-local"] {
  max-width: 50vw;
}
.list input[type="time"],
.list input[type="date"],
.list input[type="datetime-local"] {
  line-height: var(--f7-input-height);
}
.list .item-label,
.list .item-floating-label {
  width: 100%;
  vertical-align: top;
  flex-shrink: 0;
  font-size: var(--f7-label-font-size);
  font-weight: var(--f7-label-font-weight);
  line-height: var(--f7-label-line-height);
  color: var(--f7-label-text-color);
  transition-duration: 200ms;
  transition-property: transform, color;
}
.list .item-floating-label {
  --label-height: calc(var(--f7-label-font-size) * var(--f7-label-line-height));
  transform: scale(var(--f7-floating-label-scale)) translateY(calc((var(--f7-input-height) / 2 + 50%) / var(--f7-floating-label-scale)));
  color: var(--f7-input-placeholder-color);
  width: auto;
  max-width: calc(100% / var(--f7-floating-label-scale));
  pointer-events: none;
  left: var(--f7-input-padding-left);
  transform-origin: left center;
}
.list .item-floating-label ~ .item-input-wrap input::-webkit-input-placeholder,
.list .item-floating-label ~ .item-input-wrap textarea::-webkit-input-placeholder {
  opacity: 0;
  transition-duration: 100ms;
}
.list .item-floating-label ~ .item-input-wrap input::-moz-placeholder,
.list .item-floating-label ~ .item-input-wrap textarea::-moz-placeholder {
  opacity: 0;
  transition-duration: 100ms;
}
.list .item-floating-label ~ .item-input-wrap input::placeholder,
.list .item-floating-label ~ .item-input-wrap textarea::placeholder {
  opacity: 0;
  transition-duration: 100ms;
}
.list .item-floating-label ~ .item-input-wrap input.input-focused::-webkit-input-placeholder,
.list .item-floating-label ~ .item-input-wrap textarea.input-focused::-webkit-input-placeholder {
  opacity: 1;
  transition-duration: 300ms;
}
.list .item-floating-label ~ .item-input-wrap input.input-focused::-moz-placeholder,
.list .item-floating-label ~ .item-input-wrap textarea.input-focused::-moz-placeholder {
  opacity: 1;
  transition-duration: 300ms;
}
.list .item-floating-label ~ .item-input-wrap input.input-focused::placeholder,
.list .item-floating-label ~ .item-input-wrap textarea.input-focused::placeholder {
  opacity: 1;
  transition-duration: 300ms;
}
.list .item-input-with-value .item-floating-label {
  color: var(--f7-label-text-color);
}
.list .item-input-with-value .item-floating-label,
.list .item-input-focused .item-floating-label {
  transform: scale(1) translateY(0);
}
.list .item-input-wrap {
  width: 100%;
  flex-shrink: 1;
  position: relative;
}
.item-input .item-inner {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.item-input-error-message,
.input-error-message {
  font-size: var(--f7-input-error-font-size);
  line-height: var(--f7-input-error-line-height);
  color: var(--f7-input-error-text-color);
  font-weight: var(--f7-input-error-font-weight);
  display: none;
  box-sizing: border-box;
}
.item-input-info,
.input-info {
  font-size: var(--f7-input-info-font-size);
  line-height: var(--f7-input-info-line-height);
  color: var(--f7-input-info-text-color);
}
.item-input-invalid .item-input-error-message,
.input-invalid .item-input-error-message,
.item-input-invalid .input-error-message,
.input-invalid .input-error-message {
  display: block;
}
.item-input-invalid .item-input-info,
.input-invalid .item-input-info,
.item-input-invalid .input-info,
.input-invalid .input-info {
  display: none;
}
.inline-labels .item-inner,
.inline-label .item-inner {
  display: flex;
  align-items: center;
  flex-direction: row;
}
.inline-labels .item-label,
.inline-label .item-label,
.inline-labels .item-floating-label,
.inline-label .item-floating-label {
  padding-top: var(--f7-inline-label-padding-top);
  align-self: flex-start;
  width: 35%;
  font-size: var(--f7-inline-label-font-size);
  line-height: var(--f7-inline-label-line-height);
}
.inline-labels .item-label + .item-input-wrap,
.inline-label .item-label + .item-input-wrap,
.inline-labels .item-floating-label + .item-input-wrap,
.inline-label .item-floating-label + .item-input-wrap {
  margin-left: 8px;
}
.input {
  position: relative;
}
.input input,
.input select,
.input textarea {
  width: 100%;
}
.input-clear-button {
  opacity: 0;
  pointer-events: none;
  visibility: hidden;
  transition-duration: 100ms;
  position: absolute;
  top: 50%;
  border: none;
  padding: 0;
  margin: 0;
  outline: 0;
  z-index: 1;
  cursor: pointer;
  background: none;
  width: var(--f7-input-clear-button-size);
  height: var(--f7-input-clear-button-size);
  margin-top: calc(-1 * var(--f7-input-clear-button-size) / 2);
  color: var(--f7-input-clear-button-color);
  right: 0;
}
.input-clear-button:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
}
.input-clear-button:before {
  position: absolute;
  content: '';
  left: 50%;
  top: 50%;
}
.item-input-wrap .input-clear-button {
  top: calc(var(--f7-input-height) / 2);
}
.input-clear-button.active-state {
  opacity: 0.75 !important;
}
.input-with-value ~ .input-clear-button,
.item-input-with-value .input-clear-button,
.input-with-value .input-clear-button {
  opacity: 1;
  pointer-events: auto;
  visibility: visible;
}
.input-dropdown-wrap,
.input-dropdown {
  position: relative;
}
.input-dropdown-wrap:before,
.input-dropdown:before {
  content: '';
  pointer-events: none;
  position: absolute;
  top: 50%;
  margin-top: -2px;
  width: 0;
  height: 0;
  border-left: 4px solid transparent;
  border-right: 4px solid transparent;
  border-top: 5px solid #727272;
  right: 6px;
}
.input-dropdown-wrap select,
.input-dropdown select,
.input-dropdown-wrap input,
.input-dropdown input,
.input-dropdown-wrap textarea,
.input-dropdown textarea {
  padding-right: calc(20px + var(--f7-input-padding-right));
}
.input-outline:after,
.item-input-outline .item-input-wrap:after {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  border: 1px solid var(--f7-input-outline-border-color);
  border-radius: var(--f7-input-outline-border-radius);
  transition-duration: 200ms;
  pointer-events: none;
}
.input-outline.input-focused:after,
.item-input-outline.item-input-focused .item-input-wrap:after {
  border-width: 2px;
  border-color: var(--f7-input-outline-focused-border-color, var(--f7-theme-color));
}
.input-outline.input-invalid:after,
.item-input-outline.item-input-invalid .item-input-wrap:after {
  border-width: 2px;
  border-color: var(--f7-input-outline-invalid-border-color, var(--f7-input-error-text-color));
}
.input-outline input,
.item-input-outline input,
.list .item-input-outline input,
.input-outline textarea,
.item-input-outline textarea,
.list .item-input-outline textarea,
.input-outline select,
.item-input-outline select,
.list .item-input-outline select {
  border-radius: var(--f7-input-outline-border-radius);
  padding-left: var(--f7-input-outline-padding-horizontal);
  padding-right: var(--f7-input-outline-padding-horizontal);
}
.input-outline.input-dropdown:before,
.item-input-outline .input-dropdown-wrap:before {
  right: 8px;
}
.input-outline.input-dropdown input,
.item-input-outline .input-dropdown-wrap input,
.input-outline.input-dropdown textarea,
.item-input-outline .input-dropdown-wrap textarea,
.input-outline.input-dropdown select,
.item-input-outline .input-dropdown-wrap select {
  padding-right: 20px;
}
.input-outline .input-clear-button,
.item-input-outline .input-clear-button {
  right: 8px;
}
.item-input-outline {
  --f7-input-height: var(--f7-input-outline-height);
}
.item-input-outline .item-inner:after {
  display: none !important;
}
.item-input-outline .item-label {
  left: var(--f7-input-outline-padding-horizontal);
}
.inline-labels .item-input-outline .item-label,
.inline-label .item-input-outline .item-label,
.item-input-outline .inline-label .item-label,
.item-input-outline .inline-label.item-label {
  left: 0;
}
.item-input-outline .item-floating-label {
  left: calc(var(--f7-input-outline-padding-horizontal) - 4px);
  padding-left: 4px;
  padding-right: 4px;
  background: var(--f7-page-bg-color);
  z-index: 10;
  margin-top: calc(-0.5 * (var(--f7-label-font-size) * var(--f7-label-line-height)));
}
.item-input-outline.item-input-with-value .item-floating-label,
.item-input-outline.item-input-focused .item-floating-label {
  transform: scale(1) translateY(50%);
}
.item-input-outline .item-input-info,
.item-input-outline .item-input-error-message {
  padding-left: var(--f7-input-outline-padding-horizontal);
}
.block-strong .item-input-outline .item-floating-label {
  background: var(--f7-block-strong-bg-color);
}
.list .item-input-outline .item-floating-label {
  background: var(--f7-list-bg-color);
}
.ios .item-label + .item-input-wrap,
.ios .item-floating-label + .item-input-wrap {
  margin-top: 0;
}
.ios .item-input-focused .item-floating-label {
  color: var(--f7-label-text-color);
}
.ios .item-input .item-media {
  align-self: flex-start;
}
.ios .item-input-wrap {
  margin-top: calc(-1 * var(--f7-list-item-padding-vertical));
  margin-bottom: calc(-1 * var(--f7-list-item-padding-vertical));
}
.ios .inline-labels .item-label + .item-input-wrap,
.ios .inline-label .item-label + .item-input-wrap,
.ios .inline-labels .item-floating-label + .item-input-wrap,
.ios .inline-label .item-floating-label + .item-input-wrap {
  margin-top: calc(-1 * var(--f7-list-item-padding-vertical));
}
.ios .inline-labels .item-input-wrap,
.ios .inline-label .item-input-wrap {
  margin-top: calc(-1 * var(--f7-list-item-padding-vertical));
}
.ios .item-input-error-message,
.ios .item-input-info,
.ios .input-error-message,
.ios .input-info {
  position: relative;
  margin-bottom: 6px;
  margin-top: -8px;
}
.ios .item-input-focused .item-label,
.ios .item-input-focused .item-floating-label {
  color: var(--f7-label-focused-text-color, var(--f7-label-text-color));
}
.ios .item-input-focused .item-inner:after {
  background: var(--f7-input-focused-border-color, var(--f7-list-item-border-color));
}
.ios .item-input-invalid .item-label,
.ios .item-input-invalid .item-floating-label {
  color: var(--f7-label-invalid-text-color, var(--f7-label-text-color));
}
.ios .item-input-invalid .item-inner:after {
  background: var(--f7-input-invalid-border-color, var(--f7-list-item-border-color));
}
.ios .item-input-invalid input,
.ios .input-invalid input,
.ios .item-input-invalid select,
.ios .input-invalid select,
.ios .item-input-invalid textarea,
.ios .input-invalid textarea {
  color: var(--f7-input-invalid-text-color, var(--f7-input-error-text-color));
}
.ios .input-clear-button:after {
  content: 'delete_round_ios';
  font-size: calc(var(--f7-input-clear-button-size) / (14 / 10));
  line-height: 1.4;
}
.ios .input-clear-button:before {
  width: 44px;
  height: 44px;
  margin-left: -22px;
  margin-top: -22px;
}
.ios .item-input-outline .item-input-wrap,
.ios .input-outline .item-input-wrap {
  margin-top: 0;
  margin-bottom: 0;
}
.ios .item-input-outline .item-input-error-message,
.ios .input-outline .item-input-error-message,
.ios .item-input-outline .item-input-info,
.ios .input-outline .item-input-info,
.ios .item-input-outline .input-error-message,
.ios .input-outline .input-error-message,
.ios .item-input-outline .input-info,
.ios .input-outline .input-info {
  margin-top: 0;
  white-space: normal;
  overflow: hidden;
  text-overflow: ellipsis;
}
.ios .item-input-outline .item-input-info,
.ios .input-outline .item-input-info,
.ios .item-input-outline .input-info,
.ios .input-outline .input-info {
  margin-bottom: calc(-1 * var(--f7-input-info-font-size) * var(--f7-input-info-line-height));
}
.ios .item-input-outline .item-input-error-message,
.ios .input-outline .item-input-error-message,
.ios .item-input-outline .input-error-message,
.ios .input-outline .input-error-message {
  margin-bottom: calc(-1 * var(--f7-input-error-font-size) * var(--f7-input-error-line-height));
}
.ios .item-input-outline.item-input-with-info .item-input-wrap,
.ios .input-outline.item-input-with-info .item-input-wrap,
.ios .item-input-outline.input-with-info .item-input-wrap,
.ios .input-outline.input-with-info .item-input-wrap {
  margin-bottom: calc(var(--f7-input-info-font-size) * var(--f7-input-info-line-height));
}
.ios .item-input-outline.item-input-with-error-message .item-input-wrap,
.ios .input-outline.item-input-with-error-message .item-input-wrap,
.ios .item-input-outline.input-with-error-message .item-input-wrap,
.ios .input-outline.input-with-error-message .item-input-wrap {
  margin-bottom: calc(var(--f7-input-error-font-size) * var(--f7-input-error-line-height));
}
.md .item-input:not(.item-input-outline) .item-input-wrap:after,
.md .input:not(.input-outline):after {
  content: '';
  position: absolute;
  background-color: var(--f7-list-item-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.md .item-input:not(.item-input-outline) .item-input-wrap:after,
.md .input:not(.input-outline):after {
  transition-duration: 200ms;
}
.md .item-input-wrap {
  min-height: var(--f7-input-height);
}
.md .item-input .item-media {
  align-self: flex-end;
}
.md .item-input .item-inner:after {
  display: none !important;
}
.md .inline-labels .item-media,
.md .inline-label .item-media {
  align-self: flex-start;
  padding-top: 14px;
}
.md .item-input-with-error-message,
.md .item-input-with-info,
.md .input-with-error-message,
.md .input-with-info {
  padding-bottom: 20px;
}
.md .item-input-error-message,
.md .item-input-info,
.md .input-error-message,
.md .input-info {
  position: absolute;
  top: 100%;
  margin-top: 4px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  width: 100%;
  left: 0;
}
.md .item-input-focused .item-label,
.md .item-input-focused .item-floating-label {
  color: var(--f7-label-focused-text-color, var(--f7-theme-color));
}
.md .item-input-focused:not(.item-input-outline) .item-input-wrap:after,
.md .input-focused:not(.input-outline):after {
  background: var(--f7-input-focused-border-color, var(--f7-theme-color));
}
.md .item-input-invalid:not(.item-input-outline) .item-input-wrap:after,
.md .item-input-focused:not(.item-input-outline) .item-input-wrap:after,
.md .input-invalid:not(.input-outline):after,
.md .input-focused:not(.input-outline):after {
  transform: scaleY(2) !important;
}
.md .item-input-invalid:not(.item-input-outline) .item-input-wrap:after,
.md .input-invalid:not(.input-outline):after {
  background: var(--f7-input-invalid-border-color, var(--f7-input-error-text-color));
}
.md .item-input-invalid .item-label,
.md .item-input-invalid .item-floating-label {
  color: var(--f7-label-invalid-text-color, var(--f7-input-error-text-color));
}
.md .item-input-invalid input,
.md .input-invalid input,
.md .item-input-invalid select,
.md .input-invalid select,
.md .item-input-invalid textarea,
.md .input-invalid textarea {
  color: var(--f7-input-invalid-text-color, var(--f7-input-text-color));
}
.md .input-clear-button:after {
  font-size: calc(var(--f7-input-clear-button-size) / (24 / 20));
  content: 'delete_round_md';
  line-height: 1.2;
}
.md .input-clear-button:before {
  width: 48px;
  height: 48px;
  margin-left: -24px;
  margin-top: -24px;
}
.aurora .item-label + .item-input-wrap,
.aurora .item-floating-label + .item-input-wrap {
  margin-top: 0;
}
.aurora .item-input-focused .item-floating-label {
  color: var(--f7-label-text-color);
}
.aurora .item-input .item-media {
  align-self: flex-start;
}
.aurora .item-input-error-message,
.aurora .item-input-info,
.aurora .input-error-message,
.aurora .input-info {
  position: relative;
}
.aurora .item-input-focused .item-label,
.aurora .item-input-focused .item-floating-label {
  color: var(--f7-label-focused-text-color, var(--f7-label-text-color));
}
.aurora .item-input-focused .item-inner:after {
  background: var(--f7-input-focused-border-color, var(--f7-list-item-border-color));
}
.aurora .item-input-invalid .item-label,
.aurora .item-input-invalid .item-floating-label {
  color: var(--f7-label-invalid-text-color, var(--f7-label-text-color));
}
.aurora .item-input-invalid .item-inner:after {
  background: var(--f7-input-invalid-border-color, var(--f7-list-item-border-color));
}
.aurora .item-input-invalid input,
.aurora .input-invalid input,
.aurora .item-input-invalid select,
.aurora .input-invalid select,
.aurora .item-input-invalid textarea,
.aurora .input-invalid textarea {
  color: var(--f7-input-invalid-text-color, var(--f7-input-error-text-color));
}
.aurora .input-clear-button:after {
  content: 'delete_round_ios';
  font-size: calc(var(--f7-input-clear-button-size) / (14 / 10));
  line-height: 1.4;
}
.aurora .input-clear-button:before {
  width: 28px;
  height: 28px;
  margin-left: -14px;
  margin-top: -14px;
}
.aurora .item-input-outline .item-input-wrap,
.aurora .input-outline .item-input-wrap {
  margin-top: 0;
  margin-bottom: 0;
}
.aurora .item-input-outline .item-input-error-message,
.aurora .input-outline .item-input-error-message,
.aurora .item-input-outline .item-input-info,
.aurora .input-outline .item-input-info,
.aurora .item-input-outline .input-error-message,
.aurora .input-outline .input-error-message,
.aurora .item-input-outline .input-info,
.aurora .input-outline .input-info {
  margin-top: 0;
  white-space: normal;
  overflow: hidden;
  text-overflow: ellipsis;
}
.aurora .item-input-outline .item-input-info,
.aurora .input-outline .item-input-info,
.aurora .item-input-outline .input-info,
.aurora .input-outline .input-info {
  margin-bottom: calc(-1 * var(--f7-input-info-font-size) * var(--f7-input-info-line-height));
}
.aurora .item-input-outline .item-input-error-message,
.aurora .input-outline .item-input-error-message,
.aurora .item-input-outline .input-error-message,
.aurora .input-outline .input-error-message {
  margin-bottom: calc(-1 * var(--f7-input-error-font-size) * var(--f7-input-error-line-height));
}
.aurora .item-input-outline.item-input-with-info .item-input-wrap,
.aurora .input-outline.item-input-with-info .item-input-wrap,
.aurora .item-input-outline.input-with-info .item-input-wrap,
.aurora .input-outline.input-with-info .item-input-wrap {
  margin-bottom: calc(var(--f7-input-info-font-size) * var(--f7-input-info-line-height));
}
.aurora .item-input-outline.item-input-with-error-message .item-input-wrap,
.aurora .input-outline.item-input-with-error-message .item-input-wrap,
.aurora .item-input-outline.input-with-error-message .item-input-wrap,
.aurora .input-outline.input-with-error-message .item-input-wrap {
  margin-bottom: calc(var(--f7-input-error-font-size) * var(--f7-input-error-line-height));
}
/* === Checkbox === */
:root {
  /* --f7-checkbox-active-color: var(--f7-theme-color); */
  --f7-checkbox-icon-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-checkbox-inactive-color: rgba(255, 255, 255, 0.3);
}
.ios {
  --f7-checkbox-size: 22px;
  --f7-checkbox-border-radius: 50%;
  --f7-checkbox-border-width: 1px;
  --f7-checkbox-extra-margin: 0px;
  --f7-checkbox-inactive-color: #c7c7cc;
}
.md {
  --f7-checkbox-size: 18px;
  --f7-checkbox-border-radius: 2px;
  --f7-checkbox-border-width: 2px;
  --f7-checkbox-extra-margin: 22px;
  --f7-checkbox-inactive-color: #6d6d6d;
}
.aurora {
  --f7-checkbox-size: 14px;
  --f7-checkbox-border-radius: 2px;
  --f7-checkbox-border-width: 1px;
  --f7-checkbox-extra-margin: 0px;
  --f7-checkbox-inactive-color: #888;
}
.checkbox {
  position: relative;
  display: inline-block;
  vertical-align: middle;
  z-index: 1;
  background-color: transparent;
  --f7-touch-ripple-color: rgba(var(--f7-theme-color-rgb), 0.5);
}
.icon-checkbox,
.checkbox i {
  flex-shrink: 0;
  border: var(--f7-checkbox-border-width) solid var(--f7-checkbox-inactive-color);
  width: var(--f7-checkbox-size);
  height: var(--f7-checkbox-size);
  border-radius: var(--f7-checkbox-border-radius);
  box-sizing: border-box;
  position: relative;
  display: block;
}
.icon-checkbox:after,
.checkbox i:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  width: var(--f7-checkbox-size);
  height: var(--f7-checkbox-size);
  line-height: var(--f7-checkbox-size);
  left: calc(0px - var(--f7-checkbox-border-width));
  top: calc(0px - var(--f7-checkbox-border-width));
  opacity: 0;
  color: var(--f7-checkbox-icon-color);
  position: relative;
  transition-property: opacity;
}
label.item-checkbox input[type="checkbox"]:not(:checked) ~ .icon-checkbox:after,
label.item-checkbox input[type="checkbox"]:not(:checked) ~ * .icon-checkbox:after,
.checkbox input[type="checkbox"]:not(:checked) ~ i:after {
  font-size: 0;
}
label.item-checkbox input[type="checkbox"]:checked ~ .icon-checkbox,
label.item-checkbox input[type="checkbox"]:checked ~ * .icon-checkbox,
.checkbox input[type="checkbox"]:checked ~ i,
label.item-checkbox input[type="checkbox"]:indeterminate ~ .icon-checkbox,
label.item-checkbox input[type="checkbox"]:indeterminate ~ * .icon-checkbox,
.checkbox input[type="checkbox"]:indeterminate ~ i {
  border-color: var(--f7-checkbox-active-color, var(--f7-theme-color));
  background-color: var(--f7-checkbox-active-color, var(--f7-theme-color));
}
label.item-checkbox input[type="checkbox"]:checked ~ .icon-checkbox:after,
label.item-checkbox input[type="checkbox"]:checked ~ * .icon-checkbox:after,
.checkbox input[type="checkbox"]:checked ~ i:after,
label.item-checkbox input[type="checkbox"]:indeterminate ~ .icon-checkbox:after,
label.item-checkbox input[type="checkbox"]:indeterminate ~ * .icon-checkbox:after,
.checkbox input[type="checkbox"]:indeterminate ~ i:after {
  opacity: 1;
}
label.item-checkbox input[type="checkbox"]:indeterminate ~ .icon-checkbox:after,
label.item-checkbox input[type="checkbox"]:indeterminate ~ * .icon-checkbox:after,
.checkbox input[type="checkbox"]:indeterminate ~ i:after {
  font-size: 0;
  content: '';
  position: absolute;
  top: 50%;
  width: 70%;
  background: #fff;
  height: 2px;
  border-radius: 2px;
  margin-top: -1px;
  left: 15%;
  transition: 0ms;
}
label.item-checkbox,
.checkbox {
  cursor: pointer;
}
label.item-checkbox input[type="checkbox"],
.checkbox input[type="checkbox"],
label.item-checkbox input[type="radio"],
.checkbox input[type="radio"] {
  display: none;
}
label.item-checkbox {
  transition-duration: 300ms;
}
label.item-checkbox .item-content .item-media,
label.item-checkbox.item-content .item-media {
  align-self: center;
}
label.item-checkbox > .icon-checkbox {
  margin-right: calc(var(--f7-list-item-media-margin) + var(--f7-checkbox-extra-margin));
}
label.item-checkbox.active-state {
  background-color: var(--f7-list-link-pressed-bg-color);
}
label.item-checkbox.active-state:after {
  background-color: transparent;
}
label.item-checkbox.disabled,
.disabled label.item-checkbox {
  opacity: 0.55;
  pointer-events: none;
  opacity: 0.55 !important;
  pointer-events: none !important;
}
.ios .icon-checkbox:after,
.ios .checkbox i:after {
  content: 'checkbox_ios';
  font-size: 21px;
}
.ios label.item-checkbox.active-state {
  transition-duration: 0ms;
}
.ios label.item-checkbox input[type="checkbox"]:indeterminate ~ .icon-checkbox:after,
.ios label.item-checkbox input[type="checkbox"]:indeterminate ~ * .icon-checkbox:after,
.ios .checkbox input[type="checkbox"]:indeterminate ~ i:after {
  height: 1px;
  margin-top: 0px;
}
.md .icon-checkbox,
.md .checkbox i {
  transition-duration: 200ms;
}
.md .icon-checkbox:after,
.md .checkbox i:after {
  content: 'checkbox_md';
  transition-duration: 200ms;
  font-size: 15px;
}
.md label.item-checkbox {
  position: relative;
  overflow: hidden;
  z-index: 0;
}
.aurora .icon-checkbox,
.aurora .checkbox i {
  transition-duration: 150ms;
}
.aurora .icon-checkbox:after,
.aurora .checkbox i:after {
  content: 'checkbox_aurora';
  transition-duration: 150ms;
  font-size: 19px;
}
.aurora .icon-checkbox:before,
.aurora .checkbox i:before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.1);
  opacity: 0;
  transition-duration: 150ms;
}
.aurora .checkbox.active-state i:before {
  opacity: 1;
}
.aurora label.item-checkbox {
  position: relative;
  overflow: hidden;
  z-index: 0;
}
/* === Radio === */
:root {
  /*
  --f7-radio-active-color: var(--f7-theme-color);
  */
  --f7-radio-border-radius: 50%;
}
:root .theme-dark,
:root.theme-dark {
  --f7-radio-inactive-color: rgba(255, 255, 255, 0.3);
}
.ios {
  --f7-radio-size: 22px;
  --f7-radio-border-width: 1px;
  --f7-radio-extra-margin: 0px;
  --f7-radio-inactive-color: #c7c7cc;
}
.md {
  --f7-radio-size: 20px;
  --f7-radio-border-width: 2px;
  --f7-radio-extra-margin: 22px;
  --f7-radio-inactive-color: #6d6d6d;
}
.aurora {
  --f7-radio-size: 16px;
  --f7-radio-border-width: 1px;
  --f7-radio-extra-margin: 0px;
  --f7-radio-inactive-color: #888;
}
.radio {
  position: relative;
  display: inline-block;
  vertical-align: middle;
  z-index: 1;
  --f7-touch-ripple-color: rgba(var(--f7-theme-color-rgb), 0.5);
}
.icon-radio {
  width: var(--f7-radio-size);
  height: var(--f7-radio-size);
  border-radius: var(--f7-radio-border-radius);
  position: relative;
  box-sizing: border-box;
  display: block;
  flex-shrink: 0;
}
.radio .icon-radio,
.md .icon-radio,
.aurora .icon-radio {
  border: var(--f7-radio-border-width) solid var(--f7-radio-inactive-color);
}
label.item-radio,
.radio {
  cursor: pointer;
}
label.item-radio input[type="checkbox"],
.radio input[type="checkbox"],
label.item-radio input[type="radio"],
.radio input[type="radio"] {
  display: none;
}
label.item-radio {
  transition-duration: 300ms;
}
label.item-radio .item-content .item-media,
label.item-radio.item-content .item-media {
  align-self: center;
}
label.item-radio.active-state {
  background-color: var(--f7-list-link-pressed-bg-color);
}
label.item-radio.active-state:after {
  background-color: transparent;
}
label.item-radio.disabled,
.disabled label.item-radio {
  opacity: 0.55;
  pointer-events: none;
  opacity: 0.55 !important;
  pointer-events: none !important;
}
.ios .icon-radio:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  width: calc(var(--f7-radio-size) - var(--f7-radio-border-width) * 2);
  height: calc(var(--f7-radio-size) - var(--f7-radio-border-width) * 2);
  line-height: calc(var(--f7-radio-size) - var(--f7-radio-border-width) * 2 + 1px);
  font-size: 20px;
  content: 'radio_ios';
  color: var(--f7-radio-active-color, var(--f7-theme-color));
  opacity: 0;
}
.ios label.item-radio input[type="radio"]:checked ~ .icon-radio:after,
.ios label.item-radio input[type="radio"]:checked ~ * .icon-radio:after,
.ios .radio input[type="radio"]:checked ~ .icon-radio:after {
  opacity: 1;
}
.ios .radio input[type="radio"]:checked ~ .icon-radio {
  border-color: var(--f7-radio-active-color, var(--f7-theme-color));
}
.ios label.item-radio input[type="radio"] ~ .icon-radio {
  position: absolute;
  top: 50%;
  margin-top: -11px;
  right: calc(var(--f7-safe-area-right) + 10px);
}
.ios label.item-radio .item-inner {
  padding-right: calc(var(--f7-safe-area-right) + 36px);
}
.ios label.item-radio.active-state {
  transition-duration: 0ms;
}
.md .icon-radio {
  transition-duration: 200ms;
}
.md .icon-radio:after {
  content: '';
  position: absolute;
  width: 10px;
  height: 10px;
  left: 50%;
  top: 50%;
  margin-left: -5px;
  margin-top: -5px;
  background-color: var(--f7-radio-active-color, var(--f7-theme-color));
  border-radius: 50%;
  transform: scale(0);
  transition-duration: 200ms;
}
.md label.item-radio input[type="radio"]:checked ~ .icon-radio,
.md label.item-radio input[type="radio"]:checked ~ * .icon-radio,
.md .radio input[type="radio"]:checked ~ .icon-radio {
  border-color: var(--f7-radio-active-color, var(--f7-theme-color));
}
.md label.item-radio input[type="radio"]:checked ~ .icon-radio:after,
.md label.item-radio input[type="radio"]:checked ~ * .icon-radio:after,
.md .radio input[type="radio"]:checked ~ .icon-radio:after {
  background-color: var(--f7-radio-active-color, var(--f7-theme-color));
  transform: scale(1);
}
.md label.item-radio {
  position: relative;
  overflow: hidden;
  z-index: 0;
}
.md label.item-radio > .icon-radio {
  margin-right: calc(var(--f7-list-item-media-margin) + var(--f7-radio-extra-margin));
}
.aurora .icon-radio {
  transition-duration: 150ms;
  overflow: hidden;
}
.aurora .icon-radio:after {
  content: '';
  position: absolute;
  width: 6px;
  height: 6px;
  left: 50%;
  top: 50%;
  margin-left: -3px;
  margin-top: -3px;
  background-color: #fff;
  border-radius: 50%;
  transform: scale(0);
  transition-duration: 150ms;
}
.aurora .icon-radio:before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.1);
  opacity: 0;
  transition-duration: 150ms;
}
.aurora .radio.active-state i:before {
  opacity: 1;
}
.aurora label.item-radio input[type="radio"]:checked ~ .icon-radio,
.aurora label.item-radio input[type="radio"]:checked ~ * .icon-radio,
.aurora .radio input[type="radio"]:checked ~ .icon-radio {
  border-color: var(--f7-radio-active-color, var(--f7-theme-color));
  background-color: var(--f7-radio-active-color, var(--f7-theme-color));
}
.aurora label.item-radio input[type="radio"]:checked ~ .icon-radio:after,
.aurora label.item-radio input[type="radio"]:checked ~ * .icon-radio:after,
.aurora .radio input[type="radio"]:checked ~ .icon-radio:after {
  transform: scale(1);
}
.aurora label.item-radio {
  position: relative;
  overflow: hidden;
  z-index: 0;
}
.aurora label.item-radio > .icon-radio {
  margin-right: calc(var(--f7-list-item-media-margin) + var(--f7-radio-extra-margin));
}
/* === Toggle === */
:root {
  --f7-toggle-handle-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-toggle-inactive-color: #555;
}
.ios {
  --f7-toggle-width: 52px;
  --f7-toggle-height: 32px;
  --f7-toggle-border-color: #e5e5e5;
  --f7-toggle-inactive-color: #fff;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-toggle-border-color: #555;
}
.md {
  --f7-toggle-width: 36px;
  --f7-toggle-height: 14px;
  --f7-toggle-inactive-color: #b0afaf;
}
.aurora {
  --f7-toggle-width: 40px;
  --f7-toggle-height: 20px;
  --f7-toggle-inactive-color: #aaa;
}
.toggle,
.toggle-icon {
  width: var(--f7-toggle-width);
  height: var(--f7-toggle-height);
  border-radius: var(--f7-toggle-height);
}
.toggle {
  display: inline-block;
  vertical-align: middle;
  position: relative;
  box-sizing: border-box;
  align-self: center;
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
}
.toggle input[type="checkbox"] {
  display: none;
}
.toggle input[disabled] ~ .toggle-icon {
  pointer-events: none;
}
.toggle-icon {
  z-index: 0;
  margin: 0;
  padding: 0;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  border: none;
  position: relative;
  transition: 300ms;
  box-sizing: border-box;
  display: block;
  cursor: pointer;
}
.toggle-icon:before,
.toggle-icon:after {
  content: '';
}
.toggle-icon:after {
  background: var(--f7-toggle-handle-color);
  position: absolute;
  z-index: 2;
  transform: translateX(0px);
  transition-duration: 300ms;
}
.ios .toggle input[type="checkbox"]:checked + .toggle-icon {
  background: var(--f7-toggle-active-color, var(--f7-theme-color));
}
.ios .toggle input[type="checkbox"]:checked + .toggle-icon:before {
  transform: scale(0);
}
.ios .toggle input[type="checkbox"]:checked + .toggle-icon:after {
  transform: translateX(calc(var(--f7-toggle-width) - var(--f7-toggle-height)));
}
.ios .toggle-icon {
  background: var(--f7-toggle-border-color);
}
.ios .toggle-icon:before {
  position: absolute;
  left: 2px;
  top: 2px;
  width: calc(var(--f7-toggle-width) - 4px);
  height: calc(var(--f7-toggle-height) - 4px);
  border-radius: var(--f7-toggle-height);
  box-sizing: border-box;
  background: var(--f7-toggle-inactive-color);
  z-index: 1;
  transition-duration: 300ms;
  transform: scale(1);
}
.ios .toggle-icon:after {
  height: calc(var(--f7-toggle-height) - 4px);
  width: calc(var(--f7-toggle-height) - 4px);
  top: 2px;
  left: 2px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
  border-radius: calc(var(--f7-toggle-height) - 4px);
}
.ios .toggle-active-state input[type="checkbox"]:not(:checked) + .toggle-icon:before {
  transform: scale(0);
}
.ios .toggle-active-state input[type="checkbox"] + .toggle-icon:after {
  width: calc(var(--f7-toggle-height) + 4px);
}
.ios .toggle-active-state input[type="checkbox"]:checked + .toggle-icon:after {
  transform: translateX(calc(var(--f7-toggle-width) - var(--f7-toggle-height) - 8px));
}
.md .toggle input[type="checkbox"]:checked + .toggle-icon {
  background: var(--f7-toggle-active-color, rgba(var(--f7-theme-color-rgb), 0.5));
}
.md .toggle input[type="checkbox"]:checked + .toggle-icon:after {
  transform: translateX(calc(var(--f7-toggle-width) - var(--f7-toggle-height) - 6px));
  background: var(--f7-toggle-active-color, var(--f7-theme-color));
}
.md .toggle-icon {
  background: var(--f7-toggle-inactive-color);
}
.md .toggle-icon:after {
  height: calc(var(--f7-toggle-height) + 6px);
  width: calc(var(--f7-toggle-height) + 6px);
  top: -3px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.4);
  border-radius: var(--f7-toggle-height);
  left: 0;
}
.aurora .toggle input[type="checkbox"]:checked + .toggle-icon {
  background: var(--f7-toggle-active-color, var(--f7-theme-color));
}
.aurora .toggle input[type="checkbox"]:checked + .toggle-icon:after {
  transform: translateX(calc(var(--f7-toggle-width) - var(--f7-toggle-height)));
}
.aurora .toggle-icon {
  background: var(--f7-toggle-inactive-color);
}
.aurora .toggle-icon:after {
  height: calc(var(--f7-toggle-height) - 4px);
  width: calc(var(--f7-toggle-height) - 4px);
  top: 2px;
  left: 2px;
  border-radius: calc(var(--f7-toggle-height) - 4px);
}
/* === Range Slider === */
:root {
  /*
  --f7-range-bar-active-bg-color: var(--f7-theme-color);
  --f7-range-scale-bg-color: var(--f7-range-bar-bg-color);
  --f7-range-scale-substep-bg-color: var(--f7-range-bar-bg-color);
  */
  --f7-range-scale-step-height: 5px;
  --f7-range-scale-text-color: #666;
  --f7-range-scale-substep-width: 1px;
  --f7-range-scale-substep-height: 4px;
}
.ios {
  --f7-range-size: 28px;
  --f7-range-bar-bg-color: #b7b8b7;
  --f7-range-bar-size: 1px;
  --f7-range-bar-border-radius: 2px;
  --f7-range-knob-size: 28px;
  --f7-range-knob-color: #fff;
  --f7-range-knob-box-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
  --f7-range-label-size: 20px;
  --f7-range-label-text-color: #000;
  --f7-range-label-bg-color: #fff;
  --f7-range-label-font-size: 12px;
  --f7-range-label-font-weight: normal;
  --f7-range-label-border-radius: 5px;
  --f7-range-label-padding: 0px;
  --f7-range-scale-step-width: 1px;
  --f7-range-scale-font-size: 12px;
  --f7-range-scale-font-weight: 400;
  --f7-range-scale-label-offset: 4px;
}
.md {
  --f7-range-size: 20px;
  --f7-range-bar-bg-color: #b9b9b9;
  --f7-range-bar-size: 2px;
  --f7-range-bar-border-radius: 0px;
  --f7-range-knob-size: 12px;
  /*
  --f7-range-knob-color: var(--f7-theme-color);
  */
  --f7-range-knob-box-shadow: none;
  --f7-range-label-size: 26px;
  --f7-range-label-font-weight: normal;
  --f7-range-label-text-color: #fff;
  /*
  --f7-range-label-bg-color: var(--f7-theme-color);
  */
  --f7-range-label-font-size: 10px;
  --f7-range-label-border-radius: 50%;
  --f7-range-label-padding: 0px;
  --f7-range-scale-step-width: 2px;
  --f7-range-scale-font-size: 12px;
  --f7-range-scale-font-weight: 400;
  --f7-range-scale-label-offset: 4px;
}
.aurora {
  --f7-range-size: 20px;
  --f7-range-bar-bg-color: #c7c7c7;
  --f7-range-bar-size: 2px;
  --f7-range-bar-border-radius: 2px;
  --f7-range-knob-size: 16px;
  /*
  --f7-range-knob-color: var(--f7-theme-color);
  */
  --f7-range-knob-box-shadow: none;
  --f7-range-label-size: 20px;
  --f7-range-label-text-color: #fff;
  /*
  --f7-range-label-bg-color: var(--f7-theme-color);
  */
  --f7-range-label-font-size: 10px;
  --f7-range-label-font-weight: 600;
  --f7-range-label-border-radius: 4px;
  --f7-range-label-padding: 0px 4px;
  --f7-range-scale-step-width: 2px;
  --f7-range-scale-font-size: 11px;
  --f7-range-scale-font-weight: 500;
  --f7-range-scale-label-offset: 2px;
}
.range-slider {
  display: block;
  position: relative;
  align-self: center;
  cursor: pointer;
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
}
.range-slider input[type="range"] {
  display: none;
}
.range-slider.range-slider-horizontal {
  width: 100%;
  height: var(--f7-range-size);
}
.range-slider.range-slider-vertical {
  height: 100%;
  width: var(--f7-range-size);
}
.range-bar {
  position: absolute;
  overflow: hidden;
  background: var(--f7-range-bar-bg-color);
  border-radius: var(--f7-range-bar-border-radius);
}
.range-slider-vertical .range-bar {
  left: 50%;
  top: 0;
  height: 100%;
  width: var(--f7-range-bar-size);
  margin-left: calc(-1 * var(--f7-range-bar-size) / 2);
}
.range-slider-horizontal .range-bar {
  left: 0;
  top: 50%;
  width: 100%;
  height: var(--f7-range-bar-size);
  margin-top: calc(-1 * var(--f7-range-bar-size) / 2);
}
.range-bar-active {
  position: absolute;
  background: var(--f7-range-bar-active-bg-color, var(--f7-theme-color));
}
.range-slider-horizontal .range-bar-active {
  left: 0;
  top: 0;
  height: 100%;
}
.range-slider-vertical .range-bar-active {
  left: 0;
  bottom: 0;
  width: 100%;
}
.range-slider-vertical-reversed .range-bar-active {
  top: 0;
  bottom: auto;
}
.range-knob-wrap {
  z-index: 20;
  position: absolute;
  height: var(--f7-range-knob-size);
  width: var(--f7-range-knob-size);
}
.range-slider-horizontal .range-knob-wrap {
  top: 50%;
  margin-top: calc(-1 * var(--f7-range-knob-size) / 2);
  margin-left: calc(-1 * var(--f7-range-knob-size) / 2);
  left: 0;
}
.range-slider-vertical .range-knob-wrap {
  left: 50%;
  margin-left: calc(-1 * var(--f7-range-knob-size) / 2);
  bottom: 0;
  margin-bottom: calc(-1 * var(--f7-range-knob-size) / 2);
}
.range-slider-vertical-reversed .range-knob-wrap {
  bottom: auto;
  top: 0;
  margin-bottom: 0;
  margin-top: calc(-1 * var(--f7-range-knob-size) / 2);
}
.range-knob {
  box-sizing: border-box;
  border-radius: 50%;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  background: var(--f7-range-knob-color, var(--f7-range-knob-bg-color, var(--f7-theme-color)));
  box-shadow: var(--f7-range-knob-box-shadow);
}
.range-knob:after {
  content: '';
  position: absolute;
  left: 50%;
  top: 50%;
  width: 44px;
  height: 44px;
  margin-left: -22px;
  margin-top: -22px;
}
.range-knob-label {
  position: absolute;
  left: 50%;
  bottom: 100%;
  text-align: center;
  transition-duration: 120ms;
  transition-property: transform;
  box-sizing: border-box;
  transform: translateY(100%) scale(0);
  height: var(--f7-range-label-size);
  line-height: var(--f7-range-label-size);
  min-width: var(--f7-range-label-size);
  color: var(--f7-range-label-text-color);
  background-color: var(--f7-range-label-bg-color, var(--f7-theme-color));
  font-size: var(--f7-range-label-font-size);
  font-weight: var(--f7-range-label-font-weight);
  border-radius: var(--f7-range-label-border-radius);
  padding: var(--f7-range-label-padding);
}
.range-knob-active-state .range-knob-label {
  transform: translateY(0%) scale(1);
}
.range-scale {
  position: absolute;
}
.range-slider-horizontal .range-scale {
  top: 50%;
  left: 0;
  width: 100%;
  margin-top: calc(var(--f7-range-bar-size) / 2);
}
.range-slider-vertical .range-scale {
  right: 50%;
  top: 0;
  height: 100%;
  margin-right: calc(var(--f7-range-bar-size) / 2);
}
.range-scale-step {
  position: absolute;
  box-sizing: border-box;
  display: flex;
  font-size: var(--f7-range-scale-font-size);
  font-weight: var(--f7-range-scale-font-weight);
  color: var(--f7-range-scale-text-color, var(--f7-range-bar-bg-color));
  line-height: 1;
}
.range-scale-step:before {
  content: '';
  position: absolute;
  background: var(--f7-range-scale-step-bg-color, var(--f7-range-bar-bg-color));
}
.range-slider-horizontal .range-scale-step {
  justify-content: center;
  align-items: flex-start;
  width: var(--f7-range-scale-step-width);
  height: var(--f7-range-scale-step-height);
  padding-top: calc(var(--f7-range-scale-step-height) + var(--f7-range-scale-label-offset));
  top: 0;
  margin-left: calc(-1 * var(--f7-range-scale-step-width) / 2);
}
.range-slider-horizontal .range-scale-step:before {
  left: 0;
  top: 0;
  width: 100%;
  height: var(--f7-range-scale-step-height);
}
.range-slider-horizontal .range-scale-step:first-child {
  margin-left: 0;
}
.range-slider-horizontal .range-scale-step:last-child {
  margin-left: calc(-1 * var(--f7-range-scale-step-width));
}
.range-slider-vertical .range-scale-step {
  line-height: 1;
  justify-content: flex-end;
  align-items: center;
  height: var(--f7-range-scale-step-width);
  width: var(--f7-range-scale-step-height);
  padding-right: calc(var(--f7-range-scale-step-height) + var(--f7-range-scale-label-offset));
  right: 0;
  margin-bottom: calc(-1 * var(--f7-range-scale-step-width) / 2);
}
.range-slider-vertical .range-scale-step:first-child {
  margin-bottom: 0;
}
.range-slider-vertical .range-scale-step:last-child {
  margin-bottom: calc(-1 * var(--f7-range-scale-step-width));
}
.range-slider-vertical .range-scale-step:before {
  right: 0;
  top: 0;
  height: 100%;
  width: var(--f7-range-scale-step-height);
}
.range-scale-substep {
  --f7-range-scale-step-bg-color: var(--f7-range-scale-substep-bg-color, var(--f7-range-bar-bg-color));
  --f7-range-scale-step-width: var(--f7-range-scale-substep-width);
  --f7-range-scale-step-height: var(--f7-range-scale-substep-height);
}
.ios .range-knob-label {
  margin-bottom: 6px;
  transform: translateX(-50%) translateY(100%) scale(0);
}
.ios .range-knob-active-state .range-knob-label {
  transform: translateX(-50%) translateY(0%) scale(1);
}
.md .range-knob {
  transition-duration: 200ms;
  transition-property: transform, background-color;
}
.md .range-knob-active-state .range-knob {
  transform: scale(1.5);
}
.md .range-slider-min:not(.range-slider-dual) .range-knob {
  background: #fff !important;
  border: 2px solid var(--f7-range-bar-bg-color);
}
.md .range-knob-label {
  width: var(--f7-range-label-size);
  margin-left: calc(-1 * var(--f7-range-label-size) / 2);
  margin-bottom: 8px;
}
.md .range-knob-label:before {
  content: '';
  left: 50%;
  top: 0px;
  margin-left: calc(-1 * var(--f7-range-label-size) / 2);
  position: absolute;
  z-index: -1;
  width: var(--f7-range-label-size);
  height: var(--f7-range-label-size);
  background: var(--f7-range-label-bg-color, var(--f7-theme-color));
  transform: rotate(-45deg);
  border-radius: 50% 50% 50% 0;
}
.md .range-knob-active-state .range-knob-label {
  transform: translateY(0%) scale(1);
}
.md .range-slider-label .range-knob-active-state .range-knob {
  transform: scale(0);
}
.aurora .range-knob-label {
  margin-bottom: 6px;
  transform: translateX(-50%) translateY(100%) scale(0);
}
.aurora .range-knob-active-state .range-knob-label {
  transform: translateX(-50%) translateY(0%) scale(1);
}
/* === Stepper === */
:root {
  /*
  --f7-stepper-button-text-color: var(--f7-theme-color);
  --f7-stepper-button-pressed-text-color: var(--f7-button-text-color, var(--f7-theme-color));
  --f7-stepper-value-text-color: var(--f7-theme-color);
  */
  --f7-stepper-fill-button-text-color: #fff;
  /*
  --f7-stepper-fill-button-bg-color: var(--f7-theme-color);
  */
  --f7-stepper-raised-box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0,0,0,0.24);
  --f7-stepper-value-font-weight: 500;
  --f7-stepper-border-width: 2px;
}
.ios {
  --f7-stepper-height: 28px;
  --f7-stepper-border-radius: 5px;
  /*
  --f7-stepper-button-pressed-bg-color: rgba(var(--f7-theme-color-rgb), .15);
  --f7-stepper-fill-button-pressed-bg-color: var(--f7-theme-color-tint);
  */
  --f7-stepper-large-height: 44px;
  --f7-stepper-small-height: 26px;
  --f7-stepper-small-border-width: 2px;
  --f7-stepper-value-font-size: 17px;
}
.md {
  --f7-stepper-height: 36px;
  --f7-stepper-border-radius: 4px;
  /*
  --f7-stepper-fill-button-pressed-bg-color: var(--f7-theme-color-shade);
  */
  --f7-stepper-large-height: 48px;
  --f7-stepper-small-border-width: 2px;
  --f7-stepper-small-height: 28px;
  --f7-stepper-value-font-size: 14px;
  --f7-stepper-button-pressed-bg-color: rgba(0, 0, 0, 0.1);
}
.md .theme-dark,
.md.theme-dark {
  --f7-stepper-button-pressed-bg-color: rgba(255, 255, 255, 0.1);
}
.aurora {
  /*
  --f7-stepper-button-hover-bg-color: rgba(var(--f7-theme-color-rgb), .07);
  --f7-stepper-button-fill-hover-bg-color: var(--f7-theme-color-tint);
  */
  --f7-stepper-height: 28px;
  --f7-stepper-border-radius: 4px;
  /*
  --f7-stepper-button-pressed-bg-color: rgba(var(--f7-theme-color-rgb), .15);
  --f7-stepper-fill-button-pressed-bg-color: var(--f7-theme-color-shade);
  */
  --f7-stepper-large-height: 34px;
  --f7-stepper-small-border-width: 1px;
  --f7-stepper-small-height: 22px;
  --f7-stepper-value-font-size: 14px;
}
.stepper {
  display: inline-flex;
  align-items: stretch;
  height: var(--f7-stepper-height);
  border-radius: var(--f7-stepper-border-radius);
}
.stepper-button,
.stepper-button-minus,
.stepper-button-plus {
  background-color: var(--f7-stepper-button-bg-color);
  width: 40px;
  border-radius: var(--f7-stepper-border-radius);
  border: var(--f7-stepper-border-width) solid var(--f7-theme-color);
  color: var(--f7-stepper-button-text-color, var(--f7-theme-color));
  line-height: calc(var(--f7-stepper-height) - var(--f7-stepper-border-width, 0px));
  text-align: center;
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  flex-shrink: 0;
  box-sizing: border-box;
  position: relative;
  cursor: pointer;
}
.stepper-button.active-state,
.stepper-button-minus.active-state,
.stepper-button-plus.active-state {
  background-color: var(--f7-stepper-button-pressed-bg-color, rgba(var(--f7-theme-color-rgb), 0.15));
  color: var(--f7-stepper-button-pressed-text-color, var(--f7-stepper-button-text-color, var(--f7-theme-color)));
}
.stepper-button:first-child,
.stepper-button-minus:first-child,
.stepper-button-plus:first-child {
  border-radius: var(--f7-stepper-border-radius) 0 0 var(--f7-stepper-border-radius);
}
.stepper-button:last-child,
.stepper-button-minus:last-child,
.stepper-button-plus:last-child {
  border-radius: 0 var(--f7-stepper-border-radius) var(--f7-stepper-border-radius) 0;
}
.stepper-button .icon,
.stepper-button-minus .icon,
.stepper-button-plus .icon {
  pointer-events: none;
}
.stepper-button + .stepper-button,
.stepper-button-minus + .stepper-button,
.stepper-button-plus + .stepper-button,
.stepper-button + .stepper-button-minus,
.stepper-button-minus + .stepper-button-minus,
.stepper-button-plus + .stepper-button-minus,
.stepper-button + .stepper-button-plus,
.stepper-button-minus + .stepper-button-plus,
.stepper-button-plus + .stepper-button-plus {
  border-left: none;
}
.stepper-button-plus,
.stepper-button-minus {
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
}
.stepper-button-plus:after,
.stepper-button-minus:after,
.stepper-button-plus:before,
.stepper-button-minus:before {
  content: '';
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  background-color: var(--f7-stepper-button-text-color, var(--f7-theme-color));
  border-radius: 2px;
}
.stepper-button-plus:after,
.stepper-button-minus:after {
  width: 15px;
  height: 2px;
}
.stepper-button-plus:before {
  height: 15px;
  width: 2px;
}
.stepper-value {
  display: flex;
  align-content: center;
  align-items: center;
  justify-content: center;
}
.stepper-input-wrap,
.stepper-value {
  flex-shrink: 1;
  text-align: center;
  border-top: var(--f7-stepper-border-width) solid var(--f7-theme-color);
  border-bottom: var(--f7-stepper-border-width) solid var(--f7-theme-color);
}
.stepper .stepper-input-wrap input,
.stepper-value {
  width: 45px;
  color: var(--f7-stepper-value-text-color, var(--f7-theme-color));
  font-size: var(--f7-stepper-value-font-size);
  font-weight: var(--f7-stepper-value-font-weight);
  text-align: center;
}
.stepper .stepper-input-wrap input {
  height: 100%;
}
.stepper-round,
.ios .stepper-round-ios,
.md .stepper-round-md,
.aurora .stepper-round-aurora {
  --f7-stepper-border-radius: var(--f7-stepper-height);
}
.stepper-fill,
.ios .stepper-fill-ios,
.md .stepper-fill-md,
.aurora .stepper-fill-aurora {
  --f7-stepper-button-bg-color: var(--f7-stepper-fill-button-bg-color, var(--f7-theme-color));
  --f7-stepper-button-text-color: var(--f7-stepper-fill-button-text-color);
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
}
.stepper-fill .stepper-button + .stepper-button,
.ios .stepper-fill-ios .stepper-button + .stepper-button,
.md .stepper-fill-md .stepper-button + .stepper-button,
.aurora .stepper-fill-aurora .stepper-button + .stepper-button,
.stepper-raised .stepper-button + .stepper-button,
.ios .stepper-raised-ios .stepper-button + .stepper-button,
.md .stepper-raised-md .stepper-button + .stepper-button,
.aurora .stepper-raised-aurora .stepper-button + .stepper-button,
.stepper-fill .stepper-button-minus + .stepper-button-plus,
.ios .stepper-fill-ios .stepper-button-minus + .stepper-button-plus,
.md .stepper-fill-md .stepper-button-minus + .stepper-button-plus,
.aurora .stepper-fill-aurora .stepper-button-minus + .stepper-button-plus,
.stepper-raised .stepper-button-minus + .stepper-button-plus,
.ios .stepper-raised-ios .stepper-button-minus + .stepper-button-plus,
.md .stepper-raised-md .stepper-button-minus + .stepper-button-plus,
.aurora .stepper-raised-aurora .stepper-button-minus + .stepper-button-plus {
  border-left: 1px solid rgba(0, 0, 0, 0.1);
}
.stepper-fill .stepper-button + .stepper-button.active-state,
.ios .stepper-fill-ios .stepper-button + .stepper-button.active-state,
.md .stepper-fill-md .stepper-button + .stepper-button.active-state,
.aurora .stepper-fill-aurora .stepper-button + .stepper-button.active-state,
.stepper-fill .stepper-button-minus + .stepper-button-plus.active-state,
.ios .stepper-fill-ios .stepper-button-minus + .stepper-button-plus.active-state,
.md .stepper-fill-md .stepper-button-minus + .stepper-button-plus.active-state,
.aurora .stepper-fill-aurora .stepper-button-minus + .stepper-button-plus.active-state {
  border-left-color: var(--f7-stepper-button-pressed-bg-color);
}
.stepper-raised:not(.stepper-fill) .stepper-input-wrap,
.ios .stepper-raised-ios:not(.stepper-fill-ios):not(.stepper-fill) .stepper-input-wrap,
.md .stepper-raised-md:not(.stepper-fill-md):not(.stepper-fill) .stepper-input-wrap,
.aurora .stepper-raised-aurora:not(.stepper-fill-aurora):not(.stepper-fill) .stepper-input-wrap,
.stepper-raised:not(.stepper-fill) .stepper-value,
.ios .stepper-raised-ios:not(.stepper-fill-ios):not(.stepper-fill) .stepper-value,
.md .stepper-raised-md:not(.stepper-fill-md):not(.stepper-fill) .stepper-value,
.aurora .stepper-raised-aurora:not(.stepper-fill-aurora):not(.stepper-fill) .stepper-value {
  border-left: 1px solid rgba(0, 0, 0, 0.1);
  border-right: 1px solid rgba(0, 0, 0, 0.1);
}
.stepper-large,
.ios .stepper-large-ios,
.md .stepper-large-md,
.aurora .stepper-large-aurora {
  --f7-stepper-height: var(--f7-stepper-large-height);
}
.stepper-small,
.ios .stepper-small-ios,
.md .stepper-small-md,
.aurora .stepper-small-aurora {
  --f7-stepper-border-width: var(--f7-stepper-small-border-width);
  --f7-stepper-height: var(--f7-stepper-small-height);
}
.ios .stepper-fill.stepper-small-ios,
.ios .stepper-fill.stepper-small {
  --f7-stepper-button-pressed-bg-color: transparent;
  --f7-stepper-button-pressed-text-color: var(--f7-theme-color);
}
.stepper-raised,
.ios .stepper-raised-ios,
.md .stepper-raised-md,
.aurora .stepper-raised-aurora {
  --f7-stepper-border-width: 0;
  box-shadow: var(--f7-stepper-raised-box-shadow);
}
.ios .stepper-button .f7-icons,
.ios .stepper-button-minus .f7-icons,
.ios .stepper-button-plus .f7-icons {
  font-size: 22px;
}
.ios .stepper-fill,
.ios .stepper-fill-ios {
  --f7-stepper-button-pressed-bg-color: var(--f7-stepper-fill-button-pressed-bg-color, var(--f7-theme-color-tint));
}
.ios .stepper-small.stepper-raised,
.ios .stepper-small-ios.stepper-raised,
.ios .stepper-small.stepper-raised-ios,
.ios .stepper-small-ios.stepper-raised-ios {
  --f7-stepper-border-width: 0px;
}
.ios .stepper-small .stepper-button,
.ios .stepper-small-ios .stepper-button,
.ios .stepper-small .stepper-button-minus,
.ios .stepper-small-ios .stepper-button-minus,
.ios .stepper-small .stepper-button-plus,
.ios .stepper-small-ios .stepper-button-plus {
  transition-duration: 200ms;
}
.ios .stepper-small .stepper-button.active-state:after,
.ios .stepper-small-ios .stepper-button.active-state:after,
.ios .stepper-small .stepper-button-minus.active-state:after,
.ios .stepper-small-ios .stepper-button-minus.active-state:after,
.ios .stepper-small .stepper-button-plus.active-state:after,
.ios .stepper-small-ios .stepper-button-plus.active-state:after,
.ios .stepper-small .stepper-button.active-state:before,
.ios .stepper-small-ios .stepper-button.active-state:before,
.ios .stepper-small .stepper-button-minus.active-state:before,
.ios .stepper-small-ios .stepper-button-minus.active-state:before,
.ios .stepper-small .stepper-button-plus.active-state:before,
.ios .stepper-small-ios .stepper-button-plus.active-state:before {
  transition-duration: 200ms;
  background-color: var(--f7-theme-color);
}
.md .stepper-button,
.md .stepper-button-minus,
.md .stepper-button-plus {
  transition-duration: 300ms;
  transform: translate3d(0, 0, 0);
  overflow: hidden;
}
.md .stepper-fill,
.md .stepper-fill-md {
  --f7-stepper-button-pressed-bg-color: var(--f7-stepper-fill-button-pressed-bg-color, var(--f7-theme-color-shade));
}
.aurora .stepper-button,
.aurora .stepper-button-minus,
.aurora .stepper-button-plus {
  transition-duration: 100ms;
  transform: translate3d(0, 0, 0);
  overflow: hidden;
}
.aurora.device-desktop .stepper-button:not(.active-state):not(.no-hover):hover,
.aurora.device-desktop .stepper-button-minus:not(.active-state):not(.no-hover):hover,
.aurora.device-desktop .stepper-button-plus:not(.active-state):not(.no-hover):hover {
  background-color: var(--f7-stepper-button-hover-bg-color, rgba(var(--f7-theme-color-rgb), 0.07));
}
.aurora .stepper-fill,
.aurora .stepper-fill-aurora {
  --f7-stepper-button-hover-bg-color: var(--f7-stepper-button-fill-hover-bg-color, var(--f7-theme-color-tint));
  --f7-stepper-button-pressed-bg-color: var(--f7-stepper-fill-button-pressed-bg-color, var(--f7-theme-color-shade));
}
/* === Smart Select === */
.smart-select :root {
  /*
  --f7-smart-select-sheet-bg: var(--f7-list-bg-color);
  --f7-smart-select-sheet-toolbar-border-color: var(--f7-bars-border-color);
  */
}
.smart-select select {
  display: none;
}
.smart-select .item-after {
  max-width: 70%;
  overflow: hidden;
  text-overflow: ellipsis;
  position: relative;
  display: block;
}
.smart-select-sheet .page,
.smart-select-sheet .sheet-modal-inner,
.smart-select-sheet .list ul {
  background: var(--f7-smart-select-sheet-bg, var(--f7-list-bg-color));
}
.smart-select-sheet .toolbar:after {
  content: '';
  position: absolute;
  background-color: var(--f7-smart-select-sheet-toolbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.smart-select-sheet .toolbar:after {
  display: block;
}
.smart-select-sheet .list {
  margin: 0;
}
.smart-select-sheet .list ul:before,
.smart-select-sheet .list ul:after {
  display: none !important;
}
.smart-select-popover .popover-inner {
  max-height: 40vh;
}
/* === Grid === */
:root {
  --f7-grid-gap: 16px;
}
.row {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  align-items: flex-start;
  --f7-cols-per-row: 1;
}
.row > [class*="col-"],
.row > .col {
  box-sizing: border-box;
  width: calc((100% - var(--f7-grid-gap) * (var(--f7-cols-per-row) - 1)) / var(--f7-cols-per-row));
}
.row.no-gap {
  --f7-grid-gap: 0px;
}
.row .col-5 {
  --f7-cols-per-row: 20;
}
.row .col-10 {
  --f7-cols-per-row: 10;
}
.row .col-15 {
  --f7-cols-per-row: 6.66666667;
}
.row .col-20 {
  --f7-cols-per-row: 5;
}
.row .col-25 {
  --f7-cols-per-row: 4;
}
.row .col-30 {
  --f7-cols-per-row: 3.33333333;
}
.row .col-33 {
  --f7-cols-per-row: 3;
}
.row .col-35 {
  --f7-cols-per-row: 2.85714286;
}
.row .col-40 {
  --f7-cols-per-row: 2.5;
}
.row .col-45 {
  --f7-cols-per-row: 2.22222222;
}
.row .col-50 {
  --f7-cols-per-row: 2;
}
.row .col-55 {
  --f7-cols-per-row: 1.81818182;
}
.row .col-60 {
  --f7-cols-per-row: 1.66666667;
}
.row .col-65 {
  --f7-cols-per-row: 1.53846154;
}
.row .col-66 {
  --f7-cols-per-row: 1.5;
}
.row .col-70 {
  --f7-cols-per-row: 1.42857143;
}
.row .col-75 {
  --f7-cols-per-row: 1.33333333;
}
.row .col-80 {
  --f7-cols-per-row: 1.25;
}
.row .col-85 {
  --f7-cols-per-row: 1.17647059;
}
.row .col-90 {
  --f7-cols-per-row: 1.11111111;
}
.row .col-95 {
  --f7-cols-per-row: 1.05263158;
}
.row .col-100 {
  --f7-cols-per-row: 1;
}
.row .col:nth-last-child(1),
.row .col:nth-last-child(1) ~ .col {
  --f7-cols-per-row: 1;
}
.row .col:nth-last-child(2),
.row .col:nth-last-child(2) ~ .col {
  --f7-cols-per-row: 2;
}
.row .col:nth-last-child(3),
.row .col:nth-last-child(3) ~ .col {
  --f7-cols-per-row: 3;
}
.row .col:nth-last-child(4),
.row .col:nth-last-child(4) ~ .col {
  --f7-cols-per-row: 4;
}
.row .col:nth-last-child(5),
.row .col:nth-last-child(5) ~ .col {
  --f7-cols-per-row: 5;
}
.row .col:nth-last-child(6),
.row .col:nth-last-child(6) ~ .col {
  --f7-cols-per-row: 6;
}
.row .col:nth-last-child(7),
.row .col:nth-last-child(7) ~ .col {
  --f7-cols-per-row: 7;
}
.row .col:nth-last-child(8),
.row .col:nth-last-child(8) ~ .col {
  --f7-cols-per-row: 8;
}
.row .col:nth-last-child(9),
.row .col:nth-last-child(9) ~ .col {
  --f7-cols-per-row: 9;
}
.row .col:nth-last-child(10),
.row .col:nth-last-child(10) ~ .col {
  --f7-cols-per-row: 10;
}
.row .col:nth-last-child(11),
.row .col:nth-last-child(11) ~ .col {
  --f7-cols-per-row: 11;
}
.row .col:nth-last-child(12),
.row .col:nth-last-child(12) ~ .col {
  --f7-cols-per-row: 12;
}
.row .col:nth-last-child(13),
.row .col:nth-last-child(13) ~ .col {
  --f7-cols-per-row: 13;
}
.row .col:nth-last-child(14),
.row .col:nth-last-child(14) ~ .col {
  --f7-cols-per-row: 14;
}
.row .col:nth-last-child(15),
.row .col:nth-last-child(15) ~ .col {
  --f7-cols-per-row: 15;
}
.row .col:nth-last-child(16),
.row .col:nth-last-child(16) ~ .col {
  --f7-cols-per-row: 16;
}
.row .col:nth-last-child(17),
.row .col:nth-last-child(17) ~ .col {
  --f7-cols-per-row: 17;
}
.row .col:nth-last-child(18),
.row .col:nth-last-child(18) ~ .col {
  --f7-cols-per-row: 18;
}
.row .col:nth-last-child(19),
.row .col:nth-last-child(19) ~ .col {
  --f7-cols-per-row: 19;
}
.row .col:nth-last-child(20),
.row .col:nth-last-child(20) ~ .col {
  --f7-cols-per-row: 20;
}
.row .col:nth-last-child(21),
.row .col:nth-last-child(21) ~ .col {
  --f7-cols-per-row: 21;
}
.row .col:nth-last-child(22),
.row .col:nth-last-child(22) ~ .col {
  --f7-cols-per-row: 22;
}
@media (min-width: 480px) {
  .row .xsmall-5 {
    --f7-cols-per-row: 20;
  }
  .row .xsmall-10 {
    --f7-cols-per-row: 10;
  }
  .row .xsmall-15 {
    --f7-cols-per-row: 6.66666667;
  }
  .row .xsmall-20 {
    --f7-cols-per-row: 5;
  }
  .row .xsmall-25 {
    --f7-cols-per-row: 4;
  }
  .row .xsmall-30 {
    --f7-cols-per-row: 3.33333333;
  }
  .row .xsmall-33 {
    --f7-cols-per-row: 3;
  }
  .row .xsmall-35 {
    --f7-cols-per-row: 2.85714286;
  }
  .row .xsmall-40 {
    --f7-cols-per-row: 2.5;
  }
  .row .xsmall-45 {
    --f7-cols-per-row: 2.22222222;
  }
  .row .xsmall-50 {
    --f7-cols-per-row: 2;
  }
  .row .xsmall-55 {
    --f7-cols-per-row: 1.81818182;
  }
  .row .xsmall-60 {
    --f7-cols-per-row: 1.66666667;
  }
  .row .xsmall-65 {
    --f7-cols-per-row: 1.53846154;
  }
  .row .xsmall-66 {
    --f7-cols-per-row: 1.5;
  }
  .row .xsmall-70 {
    --f7-cols-per-row: 1.42857143;
  }
  .row .xsmall-75 {
    --f7-cols-per-row: 1.33333333;
  }
  .row .xsmall-80 {
    --f7-cols-per-row: 1.25;
  }
  .row .xsmall-85 {
    --f7-cols-per-row: 1.17647059;
  }
  .row .xsmall-90 {
    --f7-cols-per-row: 1.11111111;
  }
  .row .xsmall-95 {
    --f7-cols-per-row: 1.05263158;
  }
  .row .xsmall-100 {
    --f7-cols-per-row: 1;
  }
  .row .xsmall-auto:nth-last-child(1),
  .row .xsmall-auto:nth-last-child(1) ~ .xsmall-auto {
    --f7-cols-per-row: 1;
  }
  .row .xsmall-auto:nth-last-child(2),
  .row .xsmall-auto:nth-last-child(2) ~ .xsmall-auto {
    --f7-cols-per-row: 2;
  }
  .row .xsmall-auto:nth-last-child(3),
  .row .xsmall-auto:nth-last-child(3) ~ .xsmall-auto {
    --f7-cols-per-row: 3;
  }
  .row .xsmall-auto:nth-last-child(4),
  .row .xsmall-auto:nth-last-child(4) ~ .xsmall-auto {
    --f7-cols-per-row: 4;
  }
  .row .xsmall-auto:nth-last-child(5),
  .row .xsmall-auto:nth-last-child(5) ~ .xsmall-auto {
    --f7-cols-per-row: 5;
  }
  .row .xsmall-auto:nth-last-child(6),
  .row .xsmall-auto:nth-last-child(6) ~ .xsmall-auto {
    --f7-cols-per-row: 6;
  }
  .row .xsmall-auto:nth-last-child(7),
  .row .xsmall-auto:nth-last-child(7) ~ .xsmall-auto {
    --f7-cols-per-row: 7;
  }
  .row .xsmall-auto:nth-last-child(8),
  .row .xsmall-auto:nth-last-child(8) ~ .xsmall-auto {
    --f7-cols-per-row: 8;
  }
  .row .xsmall-auto:nth-last-child(9),
  .row .xsmall-auto:nth-last-child(9) ~ .xsmall-auto {
    --f7-cols-per-row: 9;
  }
  .row .xsmall-auto:nth-last-child(10),
  .row .xsmall-auto:nth-last-child(10) ~ .xsmall-auto {
    --f7-cols-per-row: 10;
  }
  .row .xsmall-auto:nth-last-child(11),
  .row .xsmall-auto:nth-last-child(11) ~ .xsmall-auto {
    --f7-cols-per-row: 11;
  }
  .row .xsmall-auto:nth-last-child(12),
  .row .xsmall-auto:nth-last-child(12) ~ .xsmall-auto {
    --f7-cols-per-row: 12;
  }
  .row .xsmall-auto:nth-last-child(13),
  .row .xsmall-auto:nth-last-child(13) ~ .xsmall-auto {
    --f7-cols-per-row: 13;
  }
  .row .xsmall-auto:nth-last-child(14),
  .row .xsmall-auto:nth-last-child(14) ~ .xsmall-auto {
    --f7-cols-per-row: 14;
  }
  .row .xsmall-auto:nth-last-child(15),
  .row .xsmall-auto:nth-last-child(15) ~ .xsmall-auto {
    --f7-cols-per-row: 15;
  }
  .row .xsmall-auto:nth-last-child(16),
  .row .xsmall-auto:nth-last-child(16) ~ .xsmall-auto {
    --f7-cols-per-row: 16;
  }
  .row .xsmall-auto:nth-last-child(17),
  .row .xsmall-auto:nth-last-child(17) ~ .xsmall-auto {
    --f7-cols-per-row: 17;
  }
  .row .xsmall-auto:nth-last-child(18),
  .row .xsmall-auto:nth-last-child(18) ~ .xsmall-auto {
    --f7-cols-per-row: 18;
  }
  .row .xsmall-auto:nth-last-child(19),
  .row .xsmall-auto:nth-last-child(19) ~ .xsmall-auto {
    --f7-cols-per-row: 19;
  }
  .row .xsmall-auto:nth-last-child(20),
  .row .xsmall-auto:nth-last-child(20) ~ .xsmall-auto {
    --f7-cols-per-row: 20;
  }
  .row .xsmall-auto:nth-last-child(21),
  .row .xsmall-auto:nth-last-child(21) ~ .xsmall-auto {
    --f7-cols-per-row: 21;
  }
  .row .xsmall-auto:nth-last-child(22),
  .row .xsmall-auto:nth-last-child(22) ~ .xsmall-auto {
    --f7-cols-per-row: 22;
  }
}
@media (min-width: 568px) {
  .row .small-5 {
    --f7-cols-per-row: 20;
  }
  .row .small-10 {
    --f7-cols-per-row: 10;
  }
  .row .small-15 {
    --f7-cols-per-row: 6.66666667;
  }
  .row .small-20 {
    --f7-cols-per-row: 5;
  }
  .row .small-25 {
    --f7-cols-per-row: 4;
  }
  .row .small-30 {
    --f7-cols-per-row: 3.33333333;
  }
  .row .small-33 {
    --f7-cols-per-row: 3;
  }
  .row .small-35 {
    --f7-cols-per-row: 2.85714286;
  }
  .row .small-40 {
    --f7-cols-per-row: 2.5;
  }
  .row .small-45 {
    --f7-cols-per-row: 2.22222222;
  }
  .row .small-50 {
    --f7-cols-per-row: 2;
  }
  .row .small-55 {
    --f7-cols-per-row: 1.81818182;
  }
  .row .small-60 {
    --f7-cols-per-row: 1.66666667;
  }
  .row .small-65 {
    --f7-cols-per-row: 1.53846154;
  }
  .row .small-66 {
    --f7-cols-per-row: 1.5;
  }
  .row .small-70 {
    --f7-cols-per-row: 1.42857143;
  }
  .row .small-75 {
    --f7-cols-per-row: 1.33333333;
  }
  .row .small-80 {
    --f7-cols-per-row: 1.25;
  }
  .row .small-85 {
    --f7-cols-per-row: 1.17647059;
  }
  .row .small-90 {
    --f7-cols-per-row: 1.11111111;
  }
  .row .small-95 {
    --f7-cols-per-row: 1.05263158;
  }
  .row .small-100 {
    --f7-cols-per-row: 1;
  }
  .row .small-auto:nth-last-child(1),
  .row .small-auto:nth-last-child(1) ~ .small-auto {
    --f7-cols-per-row: 1;
  }
  .row .small-auto:nth-last-child(2),
  .row .small-auto:nth-last-child(2) ~ .small-auto {
    --f7-cols-per-row: 2;
  }
  .row .small-auto:nth-last-child(3),
  .row .small-auto:nth-last-child(3) ~ .small-auto {
    --f7-cols-per-row: 3;
  }
  .row .small-auto:nth-last-child(4),
  .row .small-auto:nth-last-child(4) ~ .small-auto {
    --f7-cols-per-row: 4;
  }
  .row .small-auto:nth-last-child(5),
  .row .small-auto:nth-last-child(5) ~ .small-auto {
    --f7-cols-per-row: 5;
  }
  .row .small-auto:nth-last-child(6),
  .row .small-auto:nth-last-child(6) ~ .small-auto {
    --f7-cols-per-row: 6;
  }
  .row .small-auto:nth-last-child(7),
  .row .small-auto:nth-last-child(7) ~ .small-auto {
    --f7-cols-per-row: 7;
  }
  .row .small-auto:nth-last-child(8),
  .row .small-auto:nth-last-child(8) ~ .small-auto {
    --f7-cols-per-row: 8;
  }
  .row .small-auto:nth-last-child(9),
  .row .small-auto:nth-last-child(9) ~ .small-auto {
    --f7-cols-per-row: 9;
  }
  .row .small-auto:nth-last-child(10),
  .row .small-auto:nth-last-child(10) ~ .small-auto {
    --f7-cols-per-row: 10;
  }
  .row .small-auto:nth-last-child(11),
  .row .small-auto:nth-last-child(11) ~ .small-auto {
    --f7-cols-per-row: 11;
  }
  .row .small-auto:nth-last-child(12),
  .row .small-auto:nth-last-child(12) ~ .small-auto {
    --f7-cols-per-row: 12;
  }
  .row .small-auto:nth-last-child(13),
  .row .small-auto:nth-last-child(13) ~ .small-auto {
    --f7-cols-per-row: 13;
  }
  .row .small-auto:nth-last-child(14),
  .row .small-auto:nth-last-child(14) ~ .small-auto {
    --f7-cols-per-row: 14;
  }
  .row .small-auto:nth-last-child(15),
  .row .small-auto:nth-last-child(15) ~ .small-auto {
    --f7-cols-per-row: 15;
  }
  .row .small-auto:nth-last-child(16),
  .row .small-auto:nth-last-child(16) ~ .small-auto {
    --f7-cols-per-row: 16;
  }
  .row .small-auto:nth-last-child(17),
  .row .small-auto:nth-last-child(17) ~ .small-auto {
    --f7-cols-per-row: 17;
  }
  .row .small-auto:nth-last-child(18),
  .row .small-auto:nth-last-child(18) ~ .small-auto {
    --f7-cols-per-row: 18;
  }
  .row .small-auto:nth-last-child(19),
  .row .small-auto:nth-last-child(19) ~ .small-auto {
    --f7-cols-per-row: 19;
  }
  .row .small-auto:nth-last-child(20),
  .row .small-auto:nth-last-child(20) ~ .small-auto {
    --f7-cols-per-row: 20;
  }
  .row .small-auto:nth-last-child(21),
  .row .small-auto:nth-last-child(21) ~ .small-auto {
    --f7-cols-per-row: 21;
  }
  .row .small-auto:nth-last-child(22),
  .row .small-auto:nth-last-child(22) ~ .small-auto {
    --f7-cols-per-row: 22;
  }
}
@media (min-width: 768px) {
  .row .medium-5 {
    --f7-cols-per-row: 20;
  }
  .row .medium-10 {
    --f7-cols-per-row: 10;
  }
  .row .medium-15 {
    --f7-cols-per-row: 6.66666667;
  }
  .row .medium-20 {
    --f7-cols-per-row: 5;
  }
  .row .medium-25 {
    --f7-cols-per-row: 4;
  }
  .row .medium-30 {
    --f7-cols-per-row: 3.33333333;
  }
  .row .medium-33 {
    --f7-cols-per-row: 3;
  }
  .row .medium-35 {
    --f7-cols-per-row: 2.85714286;
  }
  .row .medium-40 {
    --f7-cols-per-row: 2.5;
  }
  .row .medium-45 {
    --f7-cols-per-row: 2.22222222;
  }
  .row .medium-50 {
    --f7-cols-per-row: 2;
  }
  .row .medium-55 {
    --f7-cols-per-row: 1.81818182;
  }
  .row .medium-60 {
    --f7-cols-per-row: 1.66666667;
  }
  .row .medium-65 {
    --f7-cols-per-row: 1.53846154;
  }
  .row .medium-66 {
    --f7-cols-per-row: 1.5;
  }
  .row .medium-70 {
    --f7-cols-per-row: 1.42857143;
  }
  .row .medium-75 {
    --f7-cols-per-row: 1.33333333;
  }
  .row .medium-80 {
    --f7-cols-per-row: 1.25;
  }
  .row .medium-85 {
    --f7-cols-per-row: 1.17647059;
  }
  .row .medium-90 {
    --f7-cols-per-row: 1.11111111;
  }
  .row .medium-95 {
    --f7-cols-per-row: 1.05263158;
  }
  .row .medium-100 {
    --f7-cols-per-row: 1;
  }
  .row .medium-auto:nth-last-child(1),
  .row .medium-auto:nth-last-child(1) ~ .medium-auto {
    --f7-cols-per-row: 1;
  }
  .row .medium-auto:nth-last-child(2),
  .row .medium-auto:nth-last-child(2) ~ .medium-auto {
    --f7-cols-per-row: 2;
  }
  .row .medium-auto:nth-last-child(3),
  .row .medium-auto:nth-last-child(3) ~ .medium-auto {
    --f7-cols-per-row: 3;
  }
  .row .medium-auto:nth-last-child(4),
  .row .medium-auto:nth-last-child(4) ~ .medium-auto {
    --f7-cols-per-row: 4;
  }
  .row .medium-auto:nth-last-child(5),
  .row .medium-auto:nth-last-child(5) ~ .medium-auto {
    --f7-cols-per-row: 5;
  }
  .row .medium-auto:nth-last-child(6),
  .row .medium-auto:nth-last-child(6) ~ .medium-auto {
    --f7-cols-per-row: 6;
  }
  .row .medium-auto:nth-last-child(7),
  .row .medium-auto:nth-last-child(7) ~ .medium-auto {
    --f7-cols-per-row: 7;
  }
  .row .medium-auto:nth-last-child(8),
  .row .medium-auto:nth-last-child(8) ~ .medium-auto {
    --f7-cols-per-row: 8;
  }
  .row .medium-auto:nth-last-child(9),
  .row .medium-auto:nth-last-child(9) ~ .medium-auto {
    --f7-cols-per-row: 9;
  }
  .row .medium-auto:nth-last-child(10),
  .row .medium-auto:nth-last-child(10) ~ .medium-auto {
    --f7-cols-per-row: 10;
  }
  .row .medium-auto:nth-last-child(11),
  .row .medium-auto:nth-last-child(11) ~ .medium-auto {
    --f7-cols-per-row: 11;
  }
  .row .medium-auto:nth-last-child(12),
  .row .medium-auto:nth-last-child(12) ~ .medium-auto {
    --f7-cols-per-row: 12;
  }
  .row .medium-auto:nth-last-child(13),
  .row .medium-auto:nth-last-child(13) ~ .medium-auto {
    --f7-cols-per-row: 13;
  }
  .row .medium-auto:nth-last-child(14),
  .row .medium-auto:nth-last-child(14) ~ .medium-auto {
    --f7-cols-per-row: 14;
  }
  .row .medium-auto:nth-last-child(15),
  .row .medium-auto:nth-last-child(15) ~ .medium-auto {
    --f7-cols-per-row: 15;
  }
  .row .medium-auto:nth-last-child(16),
  .row .medium-auto:nth-last-child(16) ~ .medium-auto {
    --f7-cols-per-row: 16;
  }
  .row .medium-auto:nth-last-child(17),
  .row .medium-auto:nth-last-child(17) ~ .medium-auto {
    --f7-cols-per-row: 17;
  }
  .row .medium-auto:nth-last-child(18),
  .row .medium-auto:nth-last-child(18) ~ .medium-auto {
    --f7-cols-per-row: 18;
  }
  .row .medium-auto:nth-last-child(19),
  .row .medium-auto:nth-last-child(19) ~ .medium-auto {
    --f7-cols-per-row: 19;
  }
  .row .medium-auto:nth-last-child(20),
  .row .medium-auto:nth-last-child(20) ~ .medium-auto {
    --f7-cols-per-row: 20;
  }
  .row .medium-auto:nth-last-child(21),
  .row .medium-auto:nth-last-child(21) ~ .medium-auto {
    --f7-cols-per-row: 21;
  }
  .row .medium-auto:nth-last-child(22),
  .row .medium-auto:nth-last-child(22) ~ .medium-auto {
    --f7-cols-per-row: 22;
  }
}
@media (min-width: 1024px) {
  .row .large-5 {
    --f7-cols-per-row: 20;
  }
  .row .large-10 {
    --f7-cols-per-row: 10;
  }
  .row .large-15 {
    --f7-cols-per-row: 6.66666667;
  }
  .row .large-20 {
    --f7-cols-per-row: 5;
  }
  .row .large-25 {
    --f7-cols-per-row: 4;
  }
  .row .large-30 {
    --f7-cols-per-row: 3.33333333;
  }
  .row .large-33 {
    --f7-cols-per-row: 3;
  }
  .row .large-35 {
    --f7-cols-per-row: 2.85714286;
  }
  .row .large-40 {
    --f7-cols-per-row: 2.5;
  }
  .row .large-45 {
    --f7-cols-per-row: 2.22222222;
  }
  .row .large-50 {
    --f7-cols-per-row: 2;
  }
  .row .large-55 {
    --f7-cols-per-row: 1.81818182;
  }
  .row .large-60 {
    --f7-cols-per-row: 1.66666667;
  }
  .row .large-65 {
    --f7-cols-per-row: 1.53846154;
  }
  .row .large-66 {
    --f7-cols-per-row: 1.5;
  }
  .row .large-70 {
    --f7-cols-per-row: 1.42857143;
  }
  .row .large-75 {
    --f7-cols-per-row: 1.33333333;
  }
  .row .large-80 {
    --f7-cols-per-row: 1.25;
  }
  .row .large-85 {
    --f7-cols-per-row: 1.17647059;
  }
  .row .large-90 {
    --f7-cols-per-row: 1.11111111;
  }
  .row .large-95 {
    --f7-cols-per-row: 1.05263158;
  }
  .row .large-100 {
    --f7-cols-per-row: 1;
  }
  .row .large-auto:nth-last-child(1),
  .row .large-auto:nth-last-child(1) ~ .large-auto {
    --f7-cols-per-row: 1;
  }
  .row .large-auto:nth-last-child(2),
  .row .large-auto:nth-last-child(2) ~ .large-auto {
    --f7-cols-per-row: 2;
  }
  .row .large-auto:nth-last-child(3),
  .row .large-auto:nth-last-child(3) ~ .large-auto {
    --f7-cols-per-row: 3;
  }
  .row .large-auto:nth-last-child(4),
  .row .large-auto:nth-last-child(4) ~ .large-auto {
    --f7-cols-per-row: 4;
  }
  .row .large-auto:nth-last-child(5),
  .row .large-auto:nth-last-child(5) ~ .large-auto {
    --f7-cols-per-row: 5;
  }
  .row .large-auto:nth-last-child(6),
  .row .large-auto:nth-last-child(6) ~ .large-auto {
    --f7-cols-per-row: 6;
  }
  .row .large-auto:nth-last-child(7),
  .row .large-auto:nth-last-child(7) ~ .large-auto {
    --f7-cols-per-row: 7;
  }
  .row .large-auto:nth-last-child(8),
  .row .large-auto:nth-last-child(8) ~ .large-auto {
    --f7-cols-per-row: 8;
  }
  .row .large-auto:nth-last-child(9),
  .row .large-auto:nth-last-child(9) ~ .large-auto {
    --f7-cols-per-row: 9;
  }
  .row .large-auto:nth-last-child(10),
  .row .large-auto:nth-last-child(10) ~ .large-auto {
    --f7-cols-per-row: 10;
  }
  .row .large-auto:nth-last-child(11),
  .row .large-auto:nth-last-child(11) ~ .large-auto {
    --f7-cols-per-row: 11;
  }
  .row .large-auto:nth-last-child(12),
  .row .large-auto:nth-last-child(12) ~ .large-auto {
    --f7-cols-per-row: 12;
  }
  .row .large-auto:nth-last-child(13),
  .row .large-auto:nth-last-child(13) ~ .large-auto {
    --f7-cols-per-row: 13;
  }
  .row .large-auto:nth-last-child(14),
  .row .large-auto:nth-last-child(14) ~ .large-auto {
    --f7-cols-per-row: 14;
  }
  .row .large-auto:nth-last-child(15),
  .row .large-auto:nth-last-child(15) ~ .large-auto {
    --f7-cols-per-row: 15;
  }
  .row .large-auto:nth-last-child(16),
  .row .large-auto:nth-last-child(16) ~ .large-auto {
    --f7-cols-per-row: 16;
  }
  .row .large-auto:nth-last-child(17),
  .row .large-auto:nth-last-child(17) ~ .large-auto {
    --f7-cols-per-row: 17;
  }
  .row .large-auto:nth-last-child(18),
  .row .large-auto:nth-last-child(18) ~ .large-auto {
    --f7-cols-per-row: 18;
  }
  .row .large-auto:nth-last-child(19),
  .row .large-auto:nth-last-child(19) ~ .large-auto {
    --f7-cols-per-row: 19;
  }
  .row .large-auto:nth-last-child(20),
  .row .large-auto:nth-last-child(20) ~ .large-auto {
    --f7-cols-per-row: 20;
  }
  .row .large-auto:nth-last-child(21),
  .row .large-auto:nth-last-child(21) ~ .large-auto {
    --f7-cols-per-row: 21;
  }
  .row .large-auto:nth-last-child(22),
  .row .large-auto:nth-last-child(22) ~ .large-auto {
    --f7-cols-per-row: 22;
  }
}
@media (min-width: 1200px) {
  .row .xlarge-5 {
    --f7-cols-per-row: 20;
  }
  .row .xlarge-10 {
    --f7-cols-per-row: 10;
  }
  .row .xlarge-15 {
    --f7-cols-per-row: 6.66666667;
  }
  .row .xlarge-20 {
    --f7-cols-per-row: 5;
  }
  .row .xlarge-25 {
    --f7-cols-per-row: 4;
  }
  .row .xlarge-30 {
    --f7-cols-per-row: 3.33333333;
  }
  .row .xlarge-33 {
    --f7-cols-per-row: 3;
  }
  .row .xlarge-35 {
    --f7-cols-per-row: 2.85714286;
  }
  .row .xlarge-40 {
    --f7-cols-per-row: 2.5;
  }
  .row .xlarge-45 {
    --f7-cols-per-row: 2.22222222;
  }
  .row .xlarge-50 {
    --f7-cols-per-row: 2;
  }
  .row .xlarge-55 {
    --f7-cols-per-row: 1.81818182;
  }
  .row .xlarge-60 {
    --f7-cols-per-row: 1.66666667;
  }
  .row .xlarge-65 {
    --f7-cols-per-row: 1.53846154;
  }
  .row .xlarge-66 {
    --f7-cols-per-row: 1.5;
  }
  .row .xlarge-70 {
    --f7-cols-per-row: 1.42857143;
  }
  .row .xlarge-75 {
    --f7-cols-per-row: 1.33333333;
  }
  .row .xlarge-80 {
    --f7-cols-per-row: 1.25;
  }
  .row .xlarge-85 {
    --f7-cols-per-row: 1.17647059;
  }
  .row .xlarge-90 {
    --f7-cols-per-row: 1.11111111;
  }
  .row .xlarge-95 {
    --f7-cols-per-row: 1.05263158;
  }
  .row .xlarge-100 {
    --f7-cols-per-row: 1;
  }
  .row .xlarge-auto:nth-last-child(1),
  .row .xlarge-auto:nth-last-child(1) ~ .xlarge-auto {
    --f7-cols-per-row: 1;
  }
  .row .xlarge-auto:nth-last-child(2),
  .row .xlarge-auto:nth-last-child(2) ~ .xlarge-auto {
    --f7-cols-per-row: 2;
  }
  .row .xlarge-auto:nth-last-child(3),
  .row .xlarge-auto:nth-last-child(3) ~ .xlarge-auto {
    --f7-cols-per-row: 3;
  }
  .row .xlarge-auto:nth-last-child(4),
  .row .xlarge-auto:nth-last-child(4) ~ .xlarge-auto {
    --f7-cols-per-row: 4;
  }
  .row .xlarge-auto:nth-last-child(5),
  .row .xlarge-auto:nth-last-child(5) ~ .xlarge-auto {
    --f7-cols-per-row: 5;
  }
  .row .xlarge-auto:nth-last-child(6),
  .row .xlarge-auto:nth-last-child(6) ~ .xlarge-auto {
    --f7-cols-per-row: 6;
  }
  .row .xlarge-auto:nth-last-child(7),
  .row .xlarge-auto:nth-last-child(7) ~ .xlarge-auto {
    --f7-cols-per-row: 7;
  }
  .row .xlarge-auto:nth-last-child(8),
  .row .xlarge-auto:nth-last-child(8) ~ .xlarge-auto {
    --f7-cols-per-row: 8;
  }
  .row .xlarge-auto:nth-last-child(9),
  .row .xlarge-auto:nth-last-child(9) ~ .xlarge-auto {
    --f7-cols-per-row: 9;
  }
  .row .xlarge-auto:nth-last-child(10),
  .row .xlarge-auto:nth-last-child(10) ~ .xlarge-auto {
    --f7-cols-per-row: 10;
  }
  .row .xlarge-auto:nth-last-child(11),
  .row .xlarge-auto:nth-last-child(11) ~ .xlarge-auto {
    --f7-cols-per-row: 11;
  }
  .row .xlarge-auto:nth-last-child(12),
  .row .xlarge-auto:nth-last-child(12) ~ .xlarge-auto {
    --f7-cols-per-row: 12;
  }
  .row .xlarge-auto:nth-last-child(13),
  .row .xlarge-auto:nth-last-child(13) ~ .xlarge-auto {
    --f7-cols-per-row: 13;
  }
  .row .xlarge-auto:nth-last-child(14),
  .row .xlarge-auto:nth-last-child(14) ~ .xlarge-auto {
    --f7-cols-per-row: 14;
  }
  .row .xlarge-auto:nth-last-child(15),
  .row .xlarge-auto:nth-last-child(15) ~ .xlarge-auto {
    --f7-cols-per-row: 15;
  }
  .row .xlarge-auto:nth-last-child(16),
  .row .xlarge-auto:nth-last-child(16) ~ .xlarge-auto {
    --f7-cols-per-row: 16;
  }
  .row .xlarge-auto:nth-last-child(17),
  .row .xlarge-auto:nth-last-child(17) ~ .xlarge-auto {
    --f7-cols-per-row: 17;
  }
  .row .xlarge-auto:nth-last-child(18),
  .row .xlarge-auto:nth-last-child(18) ~ .xlarge-auto {
    --f7-cols-per-row: 18;
  }
  .row .xlarge-auto:nth-last-child(19),
  .row .xlarge-auto:nth-last-child(19) ~ .xlarge-auto {
    --f7-cols-per-row: 19;
  }
  .row .xlarge-auto:nth-last-child(20),
  .row .xlarge-auto:nth-last-child(20) ~ .xlarge-auto {
    --f7-cols-per-row: 20;
  }
  .row .xlarge-auto:nth-last-child(21),
  .row .xlarge-auto:nth-last-child(21) ~ .xlarge-auto {
    --f7-cols-per-row: 21;
  }
  .row .xlarge-auto:nth-last-child(22),
  .row .xlarge-auto:nth-last-child(22) ~ .xlarge-auto {
    --f7-cols-per-row: 22;
  }
}
/* === Calendar/Datepicker === */
:root {
  --f7-calendar-height: 340px;
  --f7-calendar-sheet-landscape-height: 220px;
  --f7-calendar-popover-width: 320px;
  --f7-calendar-popover-height: 320px;
  --f7-calendar-modal-height: 420px;
  --f7-calendar-modal-max-width: 380px;
  --f7-calendar-modal-border-radius: 4px;
  /*
  --f7-calendar-header-bg-color: var(--f7-bars-bg-color);
  --f7-calendar-header-link-color: var(--f7-bars-link-color);
  --f7-calendar-header-text-color: var(--f7-bars-text-color);
  --f7-calendar-footer-bg-color: var(--f7-bars-bg-color);
  --f7-calendar-footer-border-color: var(--f7-bars-border-color);
  --f7-calendar-footer-link-color: var(--f7-bars-link-color);
  --f7-calendar-footer-text-color: var(--f7-bars-text-color);
  --f7-calendar-week-header-bg-color: var(--f7-bars-bg-color);
  --f7-calendar-week-header-text-color: var(--f7-bars-text-color);
  */
  --f7-calendar-footer-padding: 0 8px;
  --f7-calendar-week-header-font-size: 11px;
  --f7-calendar-selected-text-color: #fff;
  /*
  --f7-calendar-selected-bg-color:  var(--f7-theme-color);
  */
  --f7-calendar-prev-next-text-color: #b8b8b8;
  --f7-calendar-disabled-text-color: #d4d4d4;
  --f7-calendar-event-dot-size: 4px;
  /*
  --f7-calendar-event-bg-color: var(--f7-theme-color);
  */
  /*
  --f7-calendar-picker-selected-text-color: var(--f7-theme-color);
  */
  --f7-calendar-day-text-color: #000;
  --f7-calendar-sheet-bg-color: #fff;
  --f7-calendar-modal-bg-color: #fff;
  --f7-calendar-picker-bg-color: #fff;
  --f7-calendar-picker-pressed-bg-color: rgba(0, 0, 0, 0.1);
  --f7-calendar-picker-hover-bg-color: rgba(0, 0, 0, 0.03);
}
:root .theme-dark,
:root.theme-dark {
  --f7-calendar-sheet-border-color: var(--f7-bars-border-color);
  --f7-calendar-modal-bg-color: #121212;
  --f7-calendar-sheet-bg-color: #121212;
  --f7-calendar-picker-bg-color: #1c1c1d;
  --f7-calendar-picker-pressed-bg-color: rgba(255, 255, 255, 0.08);
  --f7-calendar-picker-hover-bg-color: rgba(255, 255, 255, 0.03);
}
.ios {
  --f7-calendar-sheet-border-color: #929499;
  --f7-calendar-header-height: 44px;
  --f7-calendar-header-font-size: 17px;
  --f7-calendar-header-font-weight: 600;
  --f7-calendar-header-padding: 0 8px;
  --f7-calendar-footer-height: 44px;
  --f7-calendar-footer-font-size: 17px;
  --f7-calendar-week-header-height: 18px;
  --f7-calendar-day-font-size: 15px;
  --f7-calendar-day-size: 30px;
  --f7-calendar-picker-font-size: 17px;
  --f7-calendar-time-selector-font-size: 17px;
  --f7-calendar-row-border-color: rgba(0, 0, 0, 0.25);
  --f7-calendar-today-text-color: #000;
  --f7-calendar-today-bg-color: #e3e3e3;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-calendar-row-border-color: var(--f7-bars-border-color);
  --f7-calendar-day-text-color: #fff;
  --f7-calendar-today-text-color: #fff;
  --f7-calendar-today-bg-color: #333;
}
.md {
  --f7-calendar-sheet-border-color: #ccc;
  --f7-calendar-header-height: 56px;
  --f7-calendar-header-font-size: 20px;
  --f7-calendar-header-font-weight: 400;
  --f7-calendar-header-padding: 0 24px;
  --f7-calendar-footer-height: 48px;
  --f7-calendar-footer-font-size: 14px;
  --f7-calendar-week-header-height: 24px;
  --f7-calendar-row-border-color: transparent;
  --f7-calendar-day-font-size: 14px;
  /*
  --f7-calendar-today-text-color: var(--f7-theme-color);
  */
  --f7-calendar-today-bg-color: none;
  --f7-calendar-day-size: 32px;
  --f7-calendar-picker-font-size: 14px;
  --f7-calendar-time-selector-font-size: 14px;
}
.md .theme-dark,
.md.theme-dark {
  --f7-calendar-day-text-color: rgba(255, 255, 255, 0.87);
}
.aurora {
  --f7-calendar-sheet-border-color: #ccc;
  --f7-calendar-header-height: 38px;
  --f7-calendar-header-font-size: 14px;
  --f7-calendar-header-font-weight: 600;
  --f7-calendar-header-padding: 0 8px;
  --f7-calendar-footer-height: 38px;
  --f7-calendar-footer-font-size: 14px;
  --f7-calendar-week-header-height: 18px;
  --f7-calendar-day-font-size: 13px;
  --f7-calendar-day-size: 30px;
  --f7-calendar-picker-font-size: 14px;
  --f7-calendar-time-selector-font-size: 14px;
  --f7-calendar-row-border-color: #e3e3e3;
  --f7-calendar-today-text-color: #000;
  --f7-calendar-today-bg-color: #e3e3e3;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-calendar-row-border-color: var(--f7-bars-border-color);
  --f7-calendar-day-text-color: #fff;
  --f7-calendar-today-text-color: #fff;
  --f7-calendar-today-bg-color: #333;
}
.calendar {
  overflow: hidden;
  height: var(--f7-calendar-height);
  width: 100%;
  display: flex;
  flex-direction: column;
}
.calendar.modal-in {
  display: flex;
}
@media (orientation: landscape) and (max-height: 415px) {
  .calendar.calendar-sheet {
    height: var(--f7-calendar-sheet-landscape-height);
  }
  .calendar.calendar-modal {
    height: calc(100vh - var(--f7-navbar-height));
  }
}
.calendar.calendar-inline,
.calendar.calendar-popover .calendar {
  position: relative;
}
.calendar-sheet {
  --f7-sheet-border-color: var(--f7-calendar-sheet-border-color);
  background: var(--f7-calendar-sheet-bg-color);
  padding-bottom: var(--f7-safe-area-bottom);
  height: calc(var(--f7-calendar-height) + var(--f7-safe-area-bottom));
}
.calendar-sheet:before {
  z-index: 600;
}
.calendar-sheet .toolbar:before,
.calendar-modal .toolbar:before,
.calendar-popover .toolbar:before {
  display: none;
}
.calendar-popover {
  width: var(--f7-calendar-popover-width);
}
.calendar-popover .calendar {
  height: var(--f7-calendar-popover-height);
  border-radius: var(--f7-popover-border-radius);
  position: relative;
}
.calendar-header {
  width: 100%;
  position: relative;
  overflow: hidden;
  flex-shrink: 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  box-sizing: border-box;
  padding: var(--f7-calendar-header-padding);
  background-color: var(--f7-calendar-header-bg-color, var(--f7-bars-bg-color));
  color: var(--f7-calendar-header-text-color, var(--f7-bars-text-color));
  height: var(--f7-calendar-header-height);
  line-height: var(--f7-calendar-header-height);
  font-size: var(--f7-calendar-header-font-size);
  font-weight: var(--f7-calendar-header-font-weight);
}
.calendar-header a {
  color: var(--f7-calendar-header-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.calendar-footer {
  width: 100%;
  flex-shrink: 0;
  padding: var(--f7-calendar-footer-padding);
  background-color: var(--f7-calendar-footer-bg-color, var(--f7-bars-bg-color));
  color: var(--f7-calendar-footer-text-color, var(--f7-bars-text-color));
  height: var(--f7-calendar-footer-height);
  font-size: var(--f7-calendar-header-font-size);
  display: flex;
  justify-content: flex-end;
  box-sizing: border-box;
  align-items: center;
  position: relative;
}
.calendar-footer a {
  color: var(--f7-calendar-footer-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.calendar-footer:before {
  content: '';
  position: absolute;
  background-color: var(--f7-calendar-footer-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.calendar-modal {
  position: absolute;
  height: var(--f7-calendar-modal-height);
  overflow: hidden;
  top: 50%;
  left: 50%;
  min-width: 300px;
  max-width: var(--f7-calendar-modal-max-width);
  transform: translate3d(-50%, 100vh, 0);
  transition-property: transform;
  display: flex;
  z-index: 13500;
  background: var(--f7-calendar-modal-bg-color);
  width: 90%;
  border-radius: var(--f7-calendar-modal-border-radius);
  box-shadow: var(--f7-elevation-24);
}
.calendar-modal.modal-in,
.calendar-modal.modal-out {
  transition-duration: 400ms;
}
.calendar-modal.modal-in {
  transform: translate3d(-50%, -50%, 0);
}
.calendar-modal.modal-out {
  transform: translate3d(-50%, 100vh, 0);
}
.calendar-week-header {
  display: flex;
  box-sizing: border-box;
  position: relative;
  font-size: var(--f7-calendar-week-header-font-size);
  background-color: var(--f7-calendar-week-header-bg-color, var(--f7-bars-bg-color));
  color: var(--f7-calendar-week-header-text-color, var(--f7-bars-text-color));
  height: var(--f7-calendar-week-header-height);
  padding-left: var(--f7-safe-area-left);
  padding-right: var(--f7-safe-area-right);
}
.calendar-week-header .calendar-week-day {
  flex-shrink: 1;
  width: calc(100% / 7);
  text-align: center;
  line-height: var(--f7-calendar-week-header-height);
}
.calendar-months {
  width: 100%;
  height: 100%;
  overflow: hidden;
  position: relative;
  flex-shrink: 10;
}
.calendar-months-wrapper {
  position: relative;
  width: 100%;
  height: 100%;
  transition: 300ms;
}
.calendar-month {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
}
.calendar-row {
  height: 16.66666667%;
  height: calc(100% / 6);
  display: flex;
  flex-shrink: 1;
  width: 100%;
  position: relative;
  box-sizing: border-box;
  padding-left: var(--f7-safe-area-left);
  padding-right: var(--f7-safe-area-right);
}
.calendar-row:before {
  content: '';
  position: absolute;
  background-color: var(--f7-calendar-row-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.calendar-modal .calendar-months:first-child .calendar-row:first-child:before,
.calendar-popover .calendar-months:first-child .calendar-row:first-child:before {
  display: none !important;
}
.calendar-day {
  flex-shrink: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  box-sizing: border-box;
  width: 14.28571429%;
  width: calc(100% / 7);
  text-align: center;
  cursor: pointer;
  z-index: 20;
  color: var(--f7-calendar-day-text-color);
  height: 100%;
  font-size: var(--f7-calendar-day-font-size);
}
.calendar-day.calendar-day-today .calendar-day-number {
  color: var(--f7-calendar-today-text-color, var(--f7-theme-color));
  background-color: var(--f7-calendar-today-bg-color);
}
.calendar-day.calendar-day-prev,
.calendar-day.calendar-day-next {
  color: var(--f7-calendar-prev-next-text-color);
}
.calendar-day.calendar-day-disabled {
  color: var(--f7-calendar-disabled-text-color);
  cursor: auto;
}
.calendar-day.calendar-day-selected .calendar-day-number {
  color: var(--f7-calendar-selected-text-color);
  background-color: var(--f7-calendar-selected-bg-color, var(--f7-theme-color));
}
.calendar-day .calendar-day-number {
  display: inline-block;
  border-radius: 50%;
  position: relative;
  width: var(--f7-calendar-day-size);
  height: var(--f7-calendar-day-size);
  line-height: var(--f7-calendar-day-size);
}
.calendar-day .calendar-day-events {
  position: absolute;
  display: flex;
  left: 0;
  width: 100%;
  top: 100%;
  align-items: center;
  justify-content: center;
  margin-top: 1px;
}
.calendar-day .calendar-day-event {
  width: var(--f7-calendar-event-dot-size);
  height: var(--f7-calendar-event-dot-size);
  border-radius: calc(var(--f7-calendar-event-dot-size) / 2);
  background-color: var(--f7-calendar-event-bg-color);
}
.calendar-day .calendar-day-event + .calendar-day-event {
  margin-left: 2px;
}
.calendar-range .calendar-day.calendar-day-selected {
  align-items: stretch;
  align-content: stretch;
}
.calendar-range .calendar-day.calendar-day-selected .calendar-day-number {
  width: 100%;
  border-radius: 0;
  height: auto;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
}
.calendar-month-selector,
.calendar-year-selector {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 50%;
  max-width: 200px;
  flex-shrink: 10;
  margin-left: auto;
  margin-right: auto;
}
.calendar-month-selector .calendar-day-number,
.calendar-year-selector .calendar-day-number {
  flex-shrink: 1;
  position: relative;
  overflow: hidden;
  text-overflow: ellipsis;
}
.calendar-month-selector a.icon-only,
.calendar-year-selector a.icon-only {
  min-width: 36px;
}
.calendar-month-picker,
.calendar-year-picker,
.calendar-time-picker {
  position: absolute;
  width: 100%;
  height: 100%;
  left: 0px;
  top: 0px;
  background: var(--f7-calendar-picker-bg-color);
  z-index: 1000;
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
}
.calendar-month-picker,
.calendar-year-picker {
  flex-wrap: wrap;
  font-size: var(--f7-calendar-picker-font-size);
  display: flex;
}
.calendar-month-picker-item,
.calendar-year-picker-item {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  overflow: hidden;
  cursor: pointer;
  transition-duration: 100ms;
  box-sizing: border-box;
}
.calendar-month-picker-item span,
.calendar-year-picker-item span {
  white-space: nowrap;
  text-overflow: ellipsis;
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  pointer-events: none;
}
.device-desktop.aurora .calendar-month-picker-item:hover,
.device-desktop.aurora .calendar-year-picker-item:hover {
  background-color: var(--f7-calendar-picker-hover-bg-color);
}
.calendar-month-picker-item.active-state,
.calendar-year-picker-item.active-state,
.device-desktop.aurora .calendar-month-picker-item.active-state,
.device-desktop.aurora .calendar-year-picker-item.active-state {
  background: var(--f7-calendar-picker-pressed-bg-color);
}
.calendar-month-picker-item {
  padding: 5px;
}
.calendar-month-picker-item:after {
  content: '';
  position: absolute;
  background-color: var(--f7-calendar-row-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.calendar-month-picker-item:before {
  content: '';
  position: absolute;
  background-color: var(--f7-calendar-row-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  width: 1px;
  height: 100%;
  transform-origin: 0% 50%;
  transform: scaleX(calc(1 / var(--f7-device-pixel-ratio)));
}
.sheet-modal .calendar-month-picker-item {
  width: 25%;
  height: calc(100% / 3);
}
.sheet-modal .calendar-month-picker-item:nth-child(4n + 1):before {
  display: none !important;
}
.sheet-modal .calendar-month-picker-item:nth-child(n + 9):after {
  display: none !important;
}
.popover .calendar-month-picker-item,
.calendar-modal .calendar-month-picker-item {
  width: calc(100% / 3);
  height: 25%;
}
.popover .calendar-month-picker-item:nth-child(3n + 1):before,
.calendar-modal .calendar-month-picker-item:nth-child(3n + 1):before {
  display: none !important;
}
.popover .calendar-month-picker-item:nth-child(n + 10):after,
.calendar-modal .calendar-month-picker-item:nth-child(n + 10):after {
  display: none !important;
}
.calendar-month-picker-item-current,
.calendar-year-picker-item-current {
  color: var(--f7-calendar-picker-selected-text-color, var(--f7-theme-color));
}
.calendar-year-picker {
  overflow: auto;
  --webkit-overflow-scrolling: touch;
}
.calendar-year-picker-item {
  height: 34px;
  line-height: 34px;
  width: 100%;
}
.calendar-year-picker-item:after {
  content: '';
  position: absolute;
  background-color: var(--f7-calendar-row-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.calendar-time-selector {
  flex-shrink: 0;
  font-size: var(--f7-calendar-time-selector-font-size);
  position: relative;
}
.calendar-time-selector:before {
  content: '';
  position: absolute;
  background-color: var(--f7-calendar-row-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.calendar-time-selector a {
  overflow: hidden;
  position: relative;
  justify-content: center;
  align-items: center;
  display: flex;
  width: 100%;
  height: 44px;
}
.calendar-time-picker {
  --f7-picker-popover-height: 100%;
  --f7-picker-inline-height: 100%;
  --f7-picker-item-selected-text-color: var(--f7-theme-color);
}
.calendar-time-picker .toolbar {
  flex-shrink: 0;
  top: 0 !important;
}
.calendar-time-picker .picker {
  height: 100%;
  display: flex;
  flex-direction: column;
}
/* === Picker === */
:root {
  --f7-picker-height: 260px;
  --f7-picker-inline-height: 200px;
  --f7-picker-popover-height: 200px;
  --f7-picker-popover-width: 280px;
  --f7-picker-landscape-height: 200px;
  --f7-picker-item-height: 36px;
  --f7-picker-item-selected-text-color: #000;
}
:root .theme-dark,
:root.theme-dark {
  --f7-picker-item-selected-text-color: #fff;
}
.ios {
  --f7-picker-column-font-size: 20px;
  --f7-picker-sheet-bg-color: #cfd5da;
  --f7-picker-divider-text-color: #000;
  --f7-picker-item-text-color: rgba(0, 0, 0, 0.45);
  --f7-picker-item-selected-border-color: rgba(0, 0, 0, 0.22);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-picker-sheet-bg-color: #1c1c1d;
  --f7-picker-divider-text-color: #fff;
  --f7-picker-item-text-color: rgba(255, 255, 255, 0.55);
  --f7-picker-item-selected-border-color: rgba(255, 255, 255, 0.06);
}
.md {
  /*
  --f7-picker-sheet-bg-color: var(--f7-sheet-bg-color);
  */
  --f7-picker-column-font-size: 20px;
  --f7-picker-divider-text-color: rgba(0, 0, 0, 0.87);
  --f7-picker-item-text-color: rgba(0, 0, 0, 0.54);
  --f7-picker-item-selected-border-color: rgba(0, 0, 0, 0.15);
}
.md .theme-dark,
.md.theme-dark {
  --f7-picker-item-text-color: rgba(255, 255, 255, 0.54);
  --f7-picker-divider-text-color: rgba(255, 255, 255, 0.87);
  --f7-picker-item-selected-border-color: rgba(255, 255, 255, 0.15);
}
.aurora {
  /*
  --f7-picker-sheet-bg-color: var(--f7-sheet-bg-color);
  */
  --f7-picker-column-font-size: 16px;
  --f7-picker-item-height: 28px;
  --f7-picker-item-text-color: #888;
  --f7-picker-divider-text-color: #000;
  --f7-picker-item-selected-border-color: rgba(0, 0, 0, 0.12);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-picker-divider-text-color: #fff;
  --f7-picker-item-selected-border-color: rgba(255, 255, 255, 0.06);
}
.picker {
  width: 100%;
  height: var(--f7-picker-height);
}
.picker.picker-inline {
  height: var(--f7-picker-inline-height);
}
.popover .picker {
  height: var(--f7-picker-popover-height);
}
@media (orientation: landscape) and (max-height: 415px) {
  .picker:not(.picker-inline) {
    height: var(--f7-picker-landscape-height);
  }
}
.picker.sheet-modal {
  background: var(--f7-picker-sheet-bg-color, var(--f7-sheet-bg-color));
}
.picker-popover {
  width: var(--f7-picker-popover-width);
}
.picker-popover .toolbar {
  background: none;
  border-radius: var(--f7-popover-border-radius) var(--f7-popover-border-radius) 0 0;
}
.picker-popover .toolbar:before {
  display: none !important;
}
.picker-popover .toolbar + .picker-columns {
  height: calc(100% - var(--f7-toolbar-height));
}
.picker-columns {
  display: flex;
  overflow: hidden;
  justify-content: center;
  padding: 0;
  text-align: right;
  height: 100%;
  position: relative;
  -webkit-mask-box-image: linear-gradient(to top, transparent, transparent 5%, white 20%, white 80%, transparent 95%, transparent);
  font-size: var(--f7-picker-column-font-size);
}
.picker-column {
  position: relative;
  max-height: 100%;
}
.picker-column.picker-column-first:before,
.picker-column.picker-column-last:after {
  height: 100%;
  width: 100vw;
  position: absolute;
  content: '';
  top: 0;
}
.picker-column.picker-column-first:before {
  right: 100%;
}
.picker-column.picker-column-last:after {
  left: 100%;
}
.picker-column.picker-column-left {
  text-align: left;
}
.picker-column.picker-column-center {
  text-align: center;
}
.picker-column.picker-column-right {
  text-align: right;
}
.picker-column.picker-column-divider {
  display: flex;
  align-items: center;
  color: var(--f7-picker-divider-text-color);
}
.picker-items {
  transition: 300ms;
  transition-timing-function: ease-out;
}
.picker-item {
  height: var(--f7-picker-item-height);
  line-height: var(--f7-picker-item-height);
  white-space: nowrap;
  position: relative;
  overflow: hidden;
  text-overflow: ellipsis;
  left: 0;
  top: 0;
  width: 100%;
  box-sizing: border-box;
  transition: 300ms;
  color: var(--f7-picker-item-text-color);
  cursor: pointer;
}
.picker-item span {
  padding: 0 10px;
}
.picker-column-absolute .picker-item {
  position: absolute;
}
.picker-item.picker-item-far {
  pointer-events: none;
}
.picker-item.picker-item-selected {
  color: var(--f7-picker-item-selected-text-color);
  transform: translate3d(0, 0, 0) rotateX(0deg);
}
.picker-center-highlight {
  height: var(--f7-picker-item-height);
  box-sizing: border-box;
  position: absolute;
  left: 0;
  width: 100%;
  top: 50%;
  margin-top: calc(-1 * var(--f7-picker-item-height) / 2);
  pointer-events: none;
}
.picker-center-highlight:before {
  content: '';
  position: absolute;
  background-color: var(--f7-picker-item-selected-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.picker-center-highlight:after {
  content: '';
  position: absolute;
  background-color: var(--f7-picker-item-selected-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.picker-3d .picker-columns {
  overflow: hidden;
  perspective: 1200px;
}
.picker-3d .picker-column,
.picker-3d .picker-items,
.picker-3d .picker-item {
  transform-style: preserve-3d;
}
.picker-3d .picker-column {
  overflow: visible;
}
.picker-3d .picker-item {
  transform-origin: center center -110px;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  transition-timing-function: ease-out;
}
/* === Infinite === */
.infinite-scroll-preloader {
  margin-left: auto;
  margin-right: auto;
  text-align: center;
}
.infinite-scroll-preloader.preloader {
  display: block;
}
.ios .infinite-scroll-preloader {
  margin-top: 35px;
  margin-bottom: 35px;
}
.ios .infinite-scroll-preloader .preloader,
.ios .infinite-scroll-preloader.preloader {
  width: 27px;
  height: 27px;
}
.md .infinite-scroll-preloader {
  margin-top: 32px;
  margin-bottom: 32px;
}
.aurora .infinite-scroll-preloader {
  margin-top: 15px;
  margin-bottom: 15px;
}
/* === PTR === */
.ios {
  --f7-ptr-preloader-size: 28px;
  --f7-ptr-size: 44px;
}
.md {
  --f7-ptr-preloader-size: 22px;
  --f7-ptr-size: 40px;
}
.aurora {
  --f7-ptr-preloader-size: 20px;
  --f7-ptr-size: 38px;
}
.ptr-preloader {
  position: relative;
  top: var(--f7-ptr-top, 0);
  height: var(--f7-ptr-size);
}
.ptr-preloader .preloader {
  position: absolute;
  left: 50%;
  width: var(--f7-ptr-preloader-size);
  height: var(--f7-ptr-preloader-size);
  margin-left: calc(-1 * var(--f7-ptr-preloader-size) / 2);
  margin-top: calc(-1 * var(--f7-ptr-preloader-size) / 2);
  top: 50%;
  visibility: hidden;
}
.ptr-bottom .ptr-preloader {
  top: auto;
  bottom: 0;
  position: fixed;
}
.ptr-with-navbar-large-transparent .ptr-preloader {
  top: calc(-1 * var(--f7-page-navbar-offset, 0px) + var(--f7-safe-area-top));
}
.ios .ptr-preloader {
  margin-top: calc(-1 * var(--f7-ptr-size));
  width: 100%;
  left: 0;
}
.ios .ptr-arrow {
  position: absolute;
  left: 50%;
  top: 50%;
  background: no-repeat center;
  z-index: 10;
  transform: rotate(0deg) translate3d(0, 0, 0);
  transition-duration: 300ms;
  transition-property: transform, opacity;
  width: 12px;
  height: 20px;
  margin-left: -6px;
  margin-top: -10px;
  visibility: visible;
  color: var(--f7-preloader-color);
}
.ios .ptr-arrow:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  width: 12px;
  height: 20px;
  line-height: 20px;
  font-size: 10px;
  content: 'ptr_arrow_ios';
}
.ios .ptr-content:not(.ptr-refreshing) .ptr-preloader .preloader {
  animation: none;
}
.ios .ptr-transitioning,
.ios .ptr-refreshing {
  transition-duration: 300ms;
  transition-property: transform;
}
.ios .ptr-refreshing {
  transform: translate3d(0, var(--f7-ptr-size), 0);
}
.ios .ptr-refreshing .ptr-arrow {
  visibility: hidden;
}
.ios .ptr-refreshing .ptr-preloader .preloader {
  visibility: visible;
}
.ios .ptr-pull-up .ptr-arrow {
  transform: rotate(180deg) translate3d(0, 0, 0);
}
.ios .ptr-no-navbar,
.ios .ptr-with-navbar-large-transparent {
  margin-top: calc(-1 * var(--f7-ptr-size));
  height: calc(100% + var(--f7-ptr-size));
}
.ios .ptr-no-navbar .ptr-preloader,
.ios .ptr-with-navbar-large-transparent .ptr-preloader {
  margin-top: 0;
}
.ios .ptr-bottom .ptr-preloader {
  margin-top: 0;
  margin-bottom: calc(-1 * var(--f7-ptr-size));
}
.ios .ptr-bottom.ptr-transitioning > *,
.ios .ptr-bottom.ptr-refreshing > * {
  transition-duration: 300ms;
  transition-property: transform;
}
.ios .ptr-bottom.ptr-refreshing {
  transform: none;
}
.ios .ptr-bottom.ptr-refreshing > * {
  transform: translate3d(0, calc(-1 * var(--f7-ptr-size)), 0);
}
.ios .ptr-bottom .ptr-arrow {
  transform: rotate(180deg) translate3d(0, 0, 0);
}
.ios .ptr-bottom.ptr-pull-up .ptr-arrow {
  transform: rotate(0deg) translate3d(0, 0, 0);
}
.ios .ptr-with-navbar-large-transparent .ptr-preloader .preloader,
.ios .ptr-with-navbar-large-transparent .ptr-preloader .ptr-arrow {
  opacity: 0;
  transition-duration: 300ms;
  transition-property: transform, opacity;
}
.ios .ptr-with-navbar-large-transparent.ptr-pull-down .ptr-preloader .preloader,
.ios .ptr-with-navbar-large-transparent.ptr-pull-up .ptr-preloader .preloader,
.ios .ptr-with-navbar-large-transparent.ptr-refreshing .ptr-preloader .preloader,
.ios .ptr-with-navbar-large-transparent.ptr-pull-down .ptr-preloader .ptr-arrow,
.ios .ptr-with-navbar-large-transparent.ptr-pull-up .ptr-preloader .ptr-arrow,
.ios .ptr-with-navbar-large-transparent.ptr-refreshing .ptr-preloader .ptr-arrow {
  opacity: 1;
}
.ios .ptr-with-navbar-large-transparent.ptr-closing .ptr-preloader .preloader,
.ios .ptr-with-navbar-large-transparent.ptr-closing .ptr-preloader .ptr-arrow {
  opacity: 0;
  transition-duration: 300ms;
}
.md {
  --f7-ptr-top: -4px;
}
.md .ptr-preloader {
  width: var(--f7-ptr-size);
  border-radius: 50%;
  background: #fff;
  margin-top: calc(-1 * var(--f7-ptr-size));
  z-index: 100;
  box-shadow: var(--f7-elevation-1);
  left: 50%;
  margin-left: calc(-1 * var(--f7-ptr-size) / 2);
}
.md .ptr-preloader .preloader .preloader-inner-gap,
.md .ptr-preloader .preloader .preloader-inner-half-circle {
  border-width: 3px;
}
.md .ptr-arrow {
  width: 22px;
  height: 22px;
  box-sizing: border-box;
  border: 3px solid var(--f7-preloader-color);
  position: absolute;
  left: 50%;
  top: 50%;
  margin-left: -11px;
  margin-top: -11px;
  border-left-color: transparent;
  border-radius: 50%;
  opacity: 1;
  transform: rotate(150deg);
}
.md .ptr-arrow:after {
  content: '';
  width: 0px;
  height: 0px;
  position: absolute;
  left: -5px;
  bottom: 0px;
  border-bottom-width: 6px;
  border-bottom-style: solid;
  border-bottom-color: inherit;
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  transform: rotate(-40deg);
}
.md .ptr-content:not(.ptr-refreshing):not(.ptr-pull-up) .ptr-preloader .preloader,
.md .ptr-content:not(.ptr-refreshing):not(.ptr-pull-up) .ptr-preloader .preloader * {
  animation: none;
}
.md .ptr-refreshing .ptr-preloader .preloader,
.md .ptr-pull-up .ptr-preloader .preloader {
  visibility: visible;
}
.md .ptr-refreshing .ptr-arrow,
.md .ptr-pull-up .ptr-arrow {
  visibility: hidden;
}
.md .ptr-refreshing .ptr-preloader {
  transform: translate3d(0, 66px, 0);
}
.md .ptr-transitioning .ptr-arrow {
  transition: 300ms;
}
.md .ptr-pull-up .ptr-arrow {
  transition: 400ms;
  transform: rotate(620deg) !important;
  opacity: 0;
}
.md .ptr-transitioning .ptr-preloader,
.md .ptr-refreshing .ptr-preloader {
  transition-duration: 300ms;
  transition-property: transform, opacity;
}
.md .ptr-bottom .ptr-preloader {
  margin-top: 0;
  margin-bottom: calc(-1 * var(--f7-ptr-size) - 4px);
}
.md .ptr-bottom.ptr-refreshing .ptr-preloader {
  transform: translate3d(0, -66px, 0);
}
.md .ptr-with-navbar-large-transparent .ptr-preloader {
  opacity: 0;
}
.md .ptr-with-navbar-large-transparent.ptr-pull-down .ptr-preloader,
.md .ptr-with-navbar-large-transparent.ptr-pull-up .ptr-preloader,
.md .ptr-with-navbar-large-transparent.ptr-refreshing .ptr-preloader {
  opacity: 1;
}
.md .ptr-with-navbar-large-transparent.ptr-closing .ptr-preloader {
  opacity: 0;
  transition-duration: 300ms;
}
.aurora .ptr-preloader {
  margin-top: calc(-1 * var(--f7-ptr-size));
  width: 100%;
  left: 0;
}
.aurora .ptr-arrow {
  position: absolute;
  left: 50%;
  top: 50%;
  background: no-repeat center;
  z-index: 10;
  transform: rotate(0deg) translate3d(0, 0, 0);
  transition-duration: 300ms;
  transition-property: transform, opacity;
  width: 12px;
  height: 20px;
  margin-left: -6px;
  margin-top: -10px;
  visibility: visible;
  color: var(--f7-preloader-color);
}
.aurora .ptr-arrow:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  width: 12px;
  height: 20px;
  line-height: 20px;
  font-size: 8px;
  content: 'ptr_arrow_ios';
}
.aurora .ptr-content:not(.ptr-refreshing) .ptr-preloader .preloader {
  animation: none;
}
.aurora .ptr-transitioning,
.aurora .ptr-refreshing {
  transition-duration: 300ms;
  transition-property: transform;
}
.aurora .ptr-refreshing {
  transform: translate3d(0, var(--f7-ptr-size), 0);
}
.aurora .ptr-refreshing .ptr-arrow {
  visibility: hidden;
}
.aurora .ptr-refreshing .ptr-preloader .preloader {
  visibility: visible;
}
.aurora .ptr-pull-up .ptr-arrow {
  transform: rotate(180deg) translate3d(0, 0, 0);
}
.aurora .ptr-no-navbar,
.aurora .ptr-with-navbar-large-transparent {
  margin-top: calc(-1 * var(--f7-ptr-size));
  height: calc(100% + var(--f7-ptr-size));
}
.aurora .ptr-no-navbar .ptr-preloader,
.aurora .ptr-with-navbar-large-transparent .ptr-preloader {
  margin-top: 0;
}
.aurora .ptr-bottom .ptr-preloader {
  margin-top: 0;
  margin-bottom: calc(-1 * var(--f7-ptr-size));
}
.aurora .ptr-bottom.ptr-transitioning > *,
.aurora .ptr-bottom.ptr-refreshing > * {
  transition-duration: 300ms;
  transition-property: transform;
}
.aurora .ptr-bottom.ptr-refreshing {
  transform: none;
}
.aurora .ptr-bottom.ptr-refreshing > * {
  transform: translate3d(0, calc(-1 * var(--f7-ptr-size)), 0);
}
.aurora .ptr-bottom .ptr-arrow {
  transform: rotate(180deg) translate3d(0, 0, 0);
}
.aurora .ptr-bottom.ptr-pull-up .ptr-arrow {
  transform: rotate(0deg) translate3d(0, 0, 0);
}
.aurora .ptr-with-navbar-large-transparent .ptr-preloader .preloader,
.aurora .ptr-with-navbar-large-transparent .ptr-preloader .ptr-arrow {
  opacity: 0;
  transition-duration: 300ms;
  transition-property: transform, opacity;
}
.aurora .ptr-with-navbar-large-transparent.ptr-pull-down .ptr-preloader .preloader,
.aurora .ptr-with-navbar-large-transparent.ptr-pull-up .ptr-preloader .preloader,
.aurora .ptr-with-navbar-large-transparent.ptr-refreshing .ptr-preloader .preloader,
.aurora .ptr-with-navbar-large-transparent.ptr-pull-down .ptr-preloader .ptr-arrow,
.aurora .ptr-with-navbar-large-transparent.ptr-pull-up .ptr-preloader .ptr-arrow,
.aurora .ptr-with-navbar-large-transparent.ptr-refreshing .ptr-preloader .ptr-arrow {
  opacity: 1;
}
.aurora .ptr-with-navbar-large-transparent.ptr-closing .ptr-preloader .preloader,
.aurora .ptr-with-navbar-large-transparent.ptr-closing .ptr-preloader .ptr-arrow {
  opacity: 0;
  transition-duration: 300ms;
}
/* === Images Lazy Loading === */
.lazy-loaded.lazy-fade-in {
  animation: lazyFadeIn 600ms;
}
@keyframes lazyFadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/* === Data Table === */
:root {
  --f7-table-head-font-size: 12px;
  --f7-table-body-font-size: 14px;
  --f7-table-footer-font-size: 12px;
  --f7-table-input-height: 24px;
  --f7-table-input-font-size: 14px;
  --f7-table-collapsible-cell-padding: 16px;
  --f7-table-link-icon-only-icon-size: 20px;
  --f7-table-sortable-icon-color: #000;
}
:root .theme-dark,
:root.theme-dark {
  --f7-table-cell-border-color: rgba(255, 255, 255, 0.15);
  --f7-table-sortable-icon-color: #fff;
  --f7-table-input-text-color: #fff;
}
.ios {
  --f7-table-head-font-weight: 600;
  --f7-table-head-cell-height: 44px;
  --f7-table-head-icon-size: 18px;
  --f7-table-body-cell-height: 44px;
  --f7-table-cell-padding-vertical: 0px;
  --f7-table-cell-padding-horizontal: 16px;
  --f7-table-edge-cell-padding-horizontal: 16px;
  --f7-table-label-cell-padding-horizontal: 16px;
  --f7-table-checkbox-cell-width: 22px;
  /* --f7-table-actions-cell-link-color: var(--f7-theme-color); */
  /* --f7-table-actions-link-color: var(--f7-theme-color); */
  --f7-table-title-font-size: 17px;
  --f7-table-title-font-weight: 600;
  --f7-table-card-header-height: 64px;
  --f7-table-footer-height: 44px;
  --f7-table-head-text-color: rgba(0, 0, 0, 0.45);
  --f7-table-cell-border-color: rgba(0, 0, 0, 0.22);
  --f7-table-selected-row-bg-color: rgba(0, 0, 0, 0.03);
  --f7-table-footer-text-color: rgba(0, 0, 0, 0.45);
  --f7-table-input-text-color: #000;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-table-head-text-color: rgba(255, 255, 255, 0.55);
  --f7-table-footer-text-color: rgba(255, 255, 255, 0.55);
  --f7-table-selected-row-bg-color: rgba(255, 255, 255, 0.08);
}
.md {
  --f7-table-head-font-weight: 500;
  --f7-table-head-cell-height: 56px;
  --f7-table-head-icon-size: 16px;
  --f7-table-body-cell-height: 48px;
  --f7-table-cell-padding-vertical: 0px;
  --f7-table-cell-padding-horizontal: 28px;
  --f7-table-edge-cell-padding-horizontal: 24px;
  --f7-table-label-cell-padding-horizontal: 24px;
  --f7-table-checkbox-cell-width: 18px;
  --f7-table-title-font-size: 20px;
  --f7-table-title-font-weight: 400;
  --f7-table-card-header-height: 64px;
  --f7-table-footer-height: 56px;
  --f7-table-head-text-color: rgba(0, 0, 0, 0.54);
  --f7-table-cell-border-color: rgba(0, 0, 0, 0.12);
  --f7-table-actions-cell-link-color: rgba(0, 0, 0, 0.54);
  --f7-table-selected-row-bg-color: #f5f5f5;
  --f7-table-actions-link-color: rgba(0, 0, 0, 0.54);
  --f7-table-footer-text-color: rgba(0, 0, 0, 0.54);
  --f7-table-input-text-color: #212121;
}
.md .theme-dark,
.md.theme-dark {
  --f7-table-head-text-color: rgba(255, 255, 255, 0.54);
  --f7-table-footer-text-color: rgba(255, 255, 255, 0.54);
  --f7-table-selected-row-bg-color: rgba(255, 255, 255, 0.05);
  --f7-table-actions-cell-link-color: rgba(255, 255, 255, 0.54);
  --f7-table-actions-link-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-table-link-icon-only-icon-size: 18px;
  --f7-table-head-font-weight: 400;
  --f7-table-head-cell-height: 32px;
  --f7-table-head-icon-size: 18px;
  --f7-table-body-cell-height: 32px;
  --f7-table-cell-padding-vertical: 5px;
  --f7-table-cell-padding-horizontal: 10px;
  --f7-table-edge-cell-padding-horizontal: 16px;
  --f7-table-label-cell-padding-horizontal: 16px;
  --f7-table-checkbox-cell-width: 22px;
  /* --f7-table-actions-cell-link-color: var(--f7-theme-color); */
  /* --f7-table-actions-link-color: var(--f7-theme-color); */
  --f7-table-title-font-size: 14px;
  --f7-table-title-font-weight: 600;
  --f7-table-card-header-height: 42px;
  --f7-table-footer-height: 32px;
  --f7-table-head-text-color: rgba(0, 0, 0, 0.6);
  --f7-table-cell-border-color: rgba(0, 0, 0, 0.12);
  --f7-table-selected-row-bg-color: rgba(0, 0, 0, 0.03);
  --f7-table-footer-text-color: rgba(0, 0, 0, 0.5);
  --f7-table-input-text-color: #000;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-table-selected-row-bg-color: rgba(255, 255, 255, 0.03);
  --f7-table-head-text-color: rgba(255, 255, 255, 0.54);
  --f7-table-footer-text-color: rgba(255, 255, 255, 0.54);
}
.data-table {
  overflow-x: auto;
}
.data-table table,
table.data-table {
  width: 100%;
  border: none;
  padding: 0;
  margin: 0;
  border-collapse: collapse;
  text-align: left;
}
.data-table thead th,
.data-table thead td {
  font-size: var(--f7-table-head-font-size);
  font-weight: var(--f7-table-head-font-weight);
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
  line-height: 16px;
  height: var(--f7-table-head-cell-height);
}
.data-table thead th:not(.sortable-cell-active),
.data-table thead td:not(.sortable-cell-active) {
  color: var(--f7-table-head-text-color);
}
.data-table thead i.icon,
.data-table thead i.f7-icons,
.data-table thead i.material-icons {
  vertical-align: top;
  font-size: var(--f7-table-head-icon-size);
}
.data-table tbody {
  font-size: var(--f7-table-body-font-size);
}
.data-table tbody th,
.data-table tbody td {
  height: var(--f7-table-body-cell-height);
}
.data-table tbody tr.data-table-row-selected,
.device-desktop .data-table tbody tr:hover {
  background: var(--f7-table-selected-row-bg-color);
}
.data-table tbody td:before,
.data-table tbody th:before {
  content: '';
  position: absolute;
  background-color: var(--f7-table-cell-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.data-table th,
.data-table td {
  --f7-table-cell-padding-left: var(--f7-table-cell-padding-horizontal);
  --f7-table-cell-padding-right: var(--f7-table-cell-padding-horizontal);
  padding-top: var(--f7-table-cell-padding-vertical);
  padding-bottom: var(--f7-table-cell-padding-vertical);
  padding-left: var(--f7-table-cell-padding-left);
  padding-right: var(--f7-table-cell-padding-right);
  position: relative;
  box-sizing: border-box;
}
.data-table th:first-child,
.data-table td:first-child {
  --f7-table-cell-padding-left: var(--f7-table-edge-cell-padding-horizontal);
}
.data-table th:last-child,
.data-table td:last-child {
  --f7-table-cell-padding-right: var(--f7-table-edge-cell-padding-horizontal);
}
.data-table th.label-cell,
.data-table td.label-cell {
  --f7-table-cell-padding-left: var(--f7-table-label-cell-padding-horizontal);
  --f7-table-cell-padding-right: var(--f7-table-label-cell-padding-horizontal);
}
.data-table th.numeric-cell,
.data-table td.numeric-cell {
  text-align: right;
}
.data-table th.checkbox-cell,
.data-table td.checkbox-cell {
  overflow: visible;
  width: var(--f7-table-checkbox-cell-width);
}
.data-table th.checkbox-cell label + span,
.data-table td.checkbox-cell label + span {
  margin-left: 8px;
}
.data-table th.checkbox-cell:first-child,
.data-table td.checkbox-cell:first-child {
  padding-right: calc(var(--f7-table-cell-padding-right) / 2);
}
.data-table th.checkbox-cell:first-child + td,
.data-table td.checkbox-cell:first-child + td,
.data-table th.checkbox-cell:first-child + th,
.data-table td.checkbox-cell:first-child + th {
  padding-left: calc(var(--f7-table-cell-padding-left) / 2);
}
.data-table th.checkbox-cell:last-child,
.data-table td.checkbox-cell:last-child {
  padding-left: calc(var(--f7-table-cell-padding-left) / 2);
}
.data-table th.actions-cell,
.data-table td.actions-cell {
  text-align: right;
  white-space: nowrap;
}
.data-table th.actions-cell a.link,
.data-table td.actions-cell a.link {
  color: var(--f7-table-actions-cell-link-color, var(--f7-theme-color));
}
.data-table th a.icon-only,
.data-table td a.icon-only,
.card .data-table th a.icon-only,
.card .data-table td a.icon-only,
.card.data-table th a.icon-only,
.card.data-table td a.icon-only {
  display: inline-block;
  vertical-align: middle;
  text-align: center;
  font-size: 0;
  min-width: 0;
}
.data-table th a.icon-only i,
.data-table td a.icon-only i,
.card .data-table th a.icon-only i,
.card .data-table td a.icon-only i,
.card.data-table th a.icon-only i,
.card.data-table td a.icon-only i {
  font-size: var(--f7-table-link-icon-only-icon-size);
  vertical-align: middle;
}
.data-table .sortable-cell:not(.input-cell) {
  cursor: pointer;
  position: relative;
}
.data-table .sortable-cell.input-cell .table-head-label {
  cursor: pointer;
  position: relative;
}
.data-table .sortable-cell:not(.numeric-cell):not(.input-cell):after,
.data-table .sortable-cell.numeric-cell:not(.input-cell):before,
.data-table .sortable-cell:not(.numeric-cell).input-cell > .table-head-label:after,
.data-table .sortable-cell.numeric-cell.input-cell > .table-head-label:before {
  content: 'arrow_bottom_md';
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  display: inline-block;
  vertical-align: top;
  width: 16px;
  height: 16px;
  color: var(--f7-table-sortable-icon-color);
  font-size: 13px;
  line-height: 16px;
  transition-duration: 300ms;
  transform: rotate(0);
  opacity: 0;
}
.device-desktop .data-table .sortable-cell:not(.sortable-cell-active):hover:after,
.device-desktop .data-table .sortable-cell:not(.sortable-cell-active) .table-head-label:hover:after,
.device-desktop .data-table .sortable-cell:not(.sortable-cell-active):hover:before,
.device-desktop .data-table .sortable-cell:not(.sortable-cell-active) .table-head-label:hover:before {
  opacity: 0.54;
}
.data-table .sortable-cell.sortable-cell-active:after,
.data-table .sortable-cell.sortable-cell-active .table-head-label:after,
.data-table .sortable-cell.sortable-cell-active:before,
.data-table .sortable-cell.sortable-cell-active .table-head-label:before {
  opacity: 0.87 !important;
}
.data-table .sortable-cell.sortable-desc:after,
.data-table .sortable-cell.sortable-desc:after,
.data-table .table-head-label:after,
.data-table .sortable-cell.sortable-desc:before,
.data-table .sortable-cell.sortable-desc:before,
.data-table .table-head-label:before {
  transform: rotate(180deg) !important;
}
.data-table.card .card-header,
.card .data-table .card-header,
.data-table.card .card-footer,
.card .data-table .card-footer {
  padding-left: var(--f7-table-edge-cell-padding-horizontal);
  padding-right: var(--f7-table-edge-cell-padding-horizontal);
}
.data-table.card .card-header,
.card .data-table .card-header {
  min-height: var(--f7-table-card-header-height);
}
.data-table.card .card-content,
.card .data-table .card-content {
  overflow-x: auto;
}
.data-table.card .card-footer,
.card .data-table .card-footer {
  min-height: var(--f7-table-footer-height);
}
.data-table .data-table-title {
  font-size: var(--f7-table-title-font-size);
  font-weight: var(--f7-table-title-font-weight);
}
.data-table .data-table-links,
.data-table .data-table-actions {
  display: flex;
}
.data-table .data-table-links .button {
  min-width: 64px;
}
.data-table .data-table-actions {
  margin-left: auto;
  align-items: center;
}
.data-table .data-table-actions a.link {
  color: var(--f7-table-actions-link-color, var(--f7-theme-color));
  min-width: 0;
}
.data-table .data-table-actions a.link.icon-only {
  line-height: 1;
  justify-content: center;
  padding: 0;
}
.data-table .data-table-header,
.data-table .data-table-header-selected {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}
.data-table .card-header > .data-table-header,
.data-table .card-header > .data-table-header-selected {
  padding-top: var(--f7-card-header-padding-vertical);
  padding-bottom: var(--f7-card-header-padding-vertical);
  height: 100%;
  padding-left: var(--f7-table-edge-cell-padding-horizontal);
  padding-right: var(--f7-table-edge-cell-padding-horizontal);
  margin-left: calc(-1 * var(--f7-table-edge-cell-padding-horizontal));
  margin-right: calc(-1 * var(--f7-table-edge-cell-padding-horizontal));
}
.data-table .data-table-header-selected {
  background: rgba(var(--f7-theme-color-rgb), 0.1);
  display: none;
}
.data-table.data-table-has-checked .data-table-header {
  display: none;
}
.data-table.data-table-has-checked .data-table-header-selected {
  display: flex;
}
.data-table .data-table-title-selected {
  font-size: 14px;
  color: var(--f7-theme-color);
}
.data-table .data-table-footer {
  display: flex;
  align-items: center;
  box-sizing: border-box;
  position: relative;
  font-size: var(--f7-table-footer-font-size);
  overflow: hidden;
  min-height: var(--f7-table-footer-height);
  color: var(--f7-table-footer-text-color);
  justify-content: flex-end;
}
.data-table .data-table-footer:before {
  content: '';
  position: absolute;
  background-color: var(--f7-table-cell-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.data-table .data-table-rows-select,
.data-table .data-table-pagination {
  display: flex;
  align-items: center;
}
.data-table .input-cell {
  padding-top: 8px;
  padding-bottom: 8px;
  height: auto;
  vertical-align: top;
}
.data-table .input-cell .table-head-label + .input {
  margin-top: 4px;
}
.data-table .input-cell .input {
  height: var(--f7-table-input-height);
}
.data-table .input-cell .input input,
.data-table .input-cell .input textarea,
.data-table .input-cell .input select {
  height: var(--f7-table-input-height);
  color: var(--f7-table-input-text-color);
  font-size: var(--f7-table-input-font-size);
}
@media (max-width: 480px) and (orientation: portrait) {
  .data-table.data-table-collapsible thead {
    display: none;
  }
  .data-table.data-table-collapsible tbody,
  .data-table.data-table-collapsible tr,
  .data-table.data-table-collapsible td {
    display: block;
  }
  .data-table.data-table-collapsible tr {
    position: relative;
  }
  .data-table.data-table-collapsible tr:before {
    content: '';
    position: absolute;
    background-color: var(--f7-table-cell-border-color);
    display: block;
    z-index: 15;
    top: 0;
    right: auto;
    bottom: auto;
    left: 0;
    height: 1px;
    width: 100%;
    transform-origin: 50% 0%;
    transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
  }
  .data-table.data-table-collapsible tr:hover {
    background-color: inherit;
  }
  .data-table.data-table-collapsible td {
    --f7-table-cell-padding-left: var(--f7-table-collapsible-cell-padding);
    --f7-table-cell-padding-right: var(--f7-table-collapsible-cell-padding);
    height: auto;
    min-height: var(--f7-table-body-cell-height);
    display: flex;
    align-content: center;
    align-items: center;
    justify-content: flex-start;
    text-align: left;
  }
  .data-table.data-table-collapsible td:before {
    display: none !important;
  }
  .data-table.data-table-collapsible td:not(.checkbox-cell):before {
    width: 40%;
    display: block !important;
    content: attr(data-collapsible-title);
    position: relative;
    height: auto;
    background: none !important;
    transform: none !important;
    font-size: var(--f7-table-head-font-size);
    font-weight: var(--f7-table-head-font-weight);
    color: var(--f7-table-head-text-color);
    margin-right: 16px;
    flex-shrink: 0;
  }
  .data-table.data-table-collapsible td.checkbox-cell {
    position: absolute;
    top: 0;
    left: 0;
  }
  .data-table.data-table-collapsible td.checkbox-cell + td {
    padding-left: 16px;
  }
  .data-table.data-table-collapsible td.checkbox-cell ~ td {
    margin-left: 32px;
  }
}
.data-table .xsmall-only,
.data-table .xsmall-landscape-only {
  display: none;
}
@media (min-width: 480px) {
  .data-table .xsmall-only {
    display: table-cell;
  }
}
@media (min-width: 480px) and (orientation: landscape) {
  .data-table .xsmall-landscape-only {
    display: table-cell;
  }
}
.data-table .small-only,
.data-table .small-landscape-only {
  display: none;
}
@media (min-width: 568px) {
  .data-table .small-only {
    display: table-cell;
  }
}
@media (min-width: 568px) and (orientation: landscape) {
  .data-table .small-landscape-only {
    display: table-cell;
  }
}
.data-table .medium-only,
.data-table .medium-landscape-only {
  display: none;
}
@media (min-width: 768px) {
  .data-table .medium-only {
    display: table-cell;
  }
}
@media (min-width: 768px) and (orientation: landscape) {
  .data-table .medium-landscape-only {
    display: table-cell;
  }
}
.data-table .large-only,
.data-table .large-landscape-only {
  display: none;
}
@media (min-width: 1024px) {
  .data-table .large-only {
    display: table-cell;
  }
}
@media (min-width: 1024px) and (orientation: landscape) {
  .data-table .large-landscape-only {
    display: table-cell;
  }
}
.data-table .xlarge-only,
.data-table .xlarge-landscape-only {
  display: none;
}
@media (min-width: 1200px) {
  .data-table .xlarge-only {
    display: table-cell;
  }
}
@media (min-width: 1200px) and (orientation: landscape) {
  .data-table .xlarge-landscape-only {
    display: table-cell;
  }
}
.ios .data-table th.actions-cell a.link + a.link,
.ios .data-table td.actions-cell a.link + a.link {
  margin-left: 16px;
}
.ios .sortable-cell:not(.numeric-cell):after {
  margin-left: 5px;
}
.ios .sortable-cell.numeric-cell:before {
  margin-right: 5px;
}
.ios .data-table-links a.link + a.link,
.ios .data-table-actions a.link + a.link,
.ios .data-table-links .button + .button,
.ios .data-table-actions .button + .button {
  margin-left: 16px;
}
.ios .data-table-actions a.link.icon-only {
  width: 44px;
  height: 44px;
}
.ios .data-table-rows-select a.link,
.ios .data-table-pagination a.link {
  width: 44px;
  height: 44px;
}
.ios .data-table-rows-select + .data-table-pagination {
  margin-left: 30px;
}
.ios .data-table-rows-select .input {
  margin-left: 20px;
}
.ios .data-table-pagination-label {
  margin-right: 16px;
}
.md .data-table th.actions-cell a.link + a.link,
.md .data-table td.actions-cell a.link + a.link {
  margin-left: 24px;
}
.md .data-table th.actions-cell a.icon-only,
.md .data-table td.actions-cell a.icon-only {
  width: 24px;
  height: 24px;
  line-height: 24px;
}
.md .sortable-cell:not(.numeric-cell):after {
  margin-left: 8px;
}
.md .sortable-cell.numeric-cell:before {
  margin-right: 8px;
}
.md .data-table-links a.link + a.link,
.md .data-table-actions a.link + a.link,
.md .data-table-links .button + .button,
.md .data-table-actions .button + .button {
  margin-left: 24px;
}
.md .data-table-actions a.link.icon-only {
  width: 24px;
  height: 24px;
  overflow: visible;
}
.md .data-table-actions a.link.icon-only.active-state {
  background: none;
}
.md .data-table-rows-select a.link,
.md .data-table-pagination a.link {
  width: 48px;
  height: 48px;
}
.md .data-table-rows-select a.link:before,
.md .data-table-pagination a.link:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .data-table-rows-select a.link.active-state:before,
.md .data-table-pagination a.link.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .data-table-rows-select + .data-table-pagination {
  margin-left: 32px;
}
.md .data-table-rows-select .input {
  margin-left: 24px;
}
.md .data-table-pagination-label {
  margin-right: 20px;
}
.md .input-cell .input-clear-button {
  transform: scale(0.8);
}
.aurora .data-table th.actions-cell a.link + a.link,
.aurora .data-table td.actions-cell a.link + a.link {
  margin-left: 10px;
}
.aurora .sortable-cell:not(.numeric-cell):after {
  margin-left: 5px;
}
.aurora .sortable-cell.numeric-cell:before {
  margin-right: 5px;
}
.aurora .data-table-links a.link + a.link,
.aurora .data-table-actions a.link + a.link,
.aurora .data-table-links .button + .button,
.aurora .data-table-actions .button + .button {
  margin-left: 10px;
}
.aurora .data-table-rows-select a.link,
.aurora .data-table-pagination a.link {
  width: 32px;
  height: 32px;
}
.aurora .data-table-rows-select + .data-table-pagination {
  margin-left: 16px;
}
.aurora .data-table-rows-select .input {
  margin-left: 10px;
}
.aurora .data-table-pagination-label {
  margin-right: 10px;
}
/* === FAB === */
:root {
  --f7-fab-margin: 16px;
  --f7-fab-text-color: #fff;
  --f7-fab-extended-text-font-size: 14px;
  --f7-fab-extended-text-padding: 0 20px;
  --f7-fab-label-bg-color: #fff;
  --f7-fab-label-text-color: #333;
  --f7-fab-label-border-radius: 4px;
  --f7-fab-label-padding: 4px 12px;
  --f7-fab-button-size: 40px;
  /* --f7-fab-pressed-bg-color: var(--f7-theme-color-shade); */
}
.ios {
  --f7-fab-size: 50px;
  --f7-fab-box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.4);
  --f7-fab-extended-size: 50px;
  --f7-fab-extended-text-font-weight: 600;
  --f7-fab-extended-text-letter-spacing: 0;
  --f7-fab-label-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.4);
  --f7-fab-label-font-size: inherit;
}
.md {
  --f7-fab-size: 56px;
  --f7-fab-box-shadow: var(--f7-elevation-6);
  --f7-fab-extended-size: 48px;
  --f7-fab-extended-text-font-weight: 500;
  --f7-fab-extended-text-letter-spacing: 0.03em;
  --f7-fab-label-box-shadow: var(--f7-elevation-3);
  --f7-fab-label-font-size: inherit;
}
.aurora {
  --f7-fab-size: 40px;
  --f7-fab-box-shadow: 0px 2px 4px rgba(0, 0, 0, 0.4);
  --f7-fab-extended-size: 38px;
  --f7-fab-extended-text-font-weight: 500;
  --f7-fab-extended-text-letter-spacing: 0;
  --f7-fab-label-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.4);
  --f7-fab-label-font-size: 12px;
}
.fab {
  position: absolute;
  z-index: 1500;
}
.fab a {
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
}
.fab[class*="fab-left"] {
  left: calc(var(--f7-fab-margin) + var(--f7-safe-area-left));
}
.fab[class*="fab-right"] {
  right: calc(var(--f7-fab-margin) + var(--f7-safe-area-right));
}
.fab[class*="-top"] {
  top: var(--f7-fab-margin);
}
.fab[class*="-bottom"] {
  bottom: calc(var(--f7-fab-margin) + var(--f7-safe-area-bottom));
}
.fab[class*="fab-center"] {
  left: 50%;
  transform: translateX(-50%);
}
.fab[class*="left-center"],
.fab[class*="right-center"] {
  top: 50%;
  transform: translateY(-50%);
}
.fab[class*="center-center"] {
  top: 50%;
  left: 50%;
  transform: translateX(-50%) translateY(-50%);
}
.fab > a,
.fab-buttons a {
  background-color: var(--f7-fab-bg-color, var(--f7-theme-color));
  width: var(--f7-fab-size);
  height: var(--f7-fab-size);
  box-shadow: var(--f7-fab-box-shadow);
  border-radius: calc(var(--f7-fab-size) / 2);
  position: relative;
  transition-duration: 300ms;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  z-index: 1;
  color: var(--f7-fab-text-color);
}
.fab > a.active-state,
.fab-buttons a.active-state {
  background-color: var(--f7-fab-pressed-bg-color, var(--f7-theme-color-shade));
}
.fab > a i {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0) rotate(0deg) scale(1);
  transition: 300ms;
}
.fab > a i + i {
  transform: translate3d(-50%, -50%, 0) rotate(-90deg) scale(0.5);
  opacity: 0;
}
.fab-buttons a {
  border-radius: calc(var(--f7-fab-button-size) / 2);
  width: var(--f7-fab-button-size);
  height: var(--f7-fab-button-size);
}
.fab-buttons {
  display: flex;
  visibility: hidden;
  pointer-events: none;
  position: absolute;
}
.fab-buttons a {
  opacity: 0;
}
.fab-opened:not(.fab-morph) > a i {
  transform: translate3d(-50%, -50%, 0) rotate(90deg) scale(0.5);
  opacity: 0;
}
.fab-opened:not(.fab-morph) > a i + i {
  transform: translate3d(-50%, -50%, 0) rotate(0deg) scale(1);
  opacity: 1;
}
.fab-opened .fab-buttons {
  visibility: visible;
  pointer-events: auto;
}
.fab-opened .fab-buttons a {
  opacity: 1;
  transform: translate3d(0, 0px, 0) scale(1) !important;
}
.fab-opened .fab-buttons a:nth-child(2) {
  transition-delay: 50ms;
}
.fab-opened .fab-buttons a:nth-child(3) {
  transition-delay: 100ms;
}
.fab-opened .fab-buttons a:nth-child(4) {
  transition-delay: 150ms;
}
.fab-opened .fab-buttons a:nth-child(5) {
  transition-delay: 200ms;
}
.fab-opened .fab-buttons a:nth-child(6) {
  transition-delay: 250ms;
}
.fab-buttons-top,
.fab-buttons-bottom {
  left: 50%;
  width: var(--f7-fab-button-size);
  margin-left: calc(-1 * var(--f7-fab-button-size) / 2);
}
.fab-buttons-top {
  bottom: 100%;
  margin-bottom: 16px;
  flex-direction: column-reverse;
}
.fab-buttons-top a {
  transform: translate3d(0, 8px, 0) scale(0.3);
  transform-origin: center bottom;
}
.fab-buttons-top a + a {
  margin-bottom: 16px;
}
.fab-buttons-bottom {
  top: 100%;
  margin-top: 16px;
  flex-direction: column;
}
.fab-buttons-bottom a {
  transform: translate3d(0, -8px, 0) scale(0.3);
  transform-origin: center top;
}
.fab-buttons-bottom a + a {
  margin-top: 16px;
}
.fab-buttons-left,
.fab-buttons-right {
  top: 50%;
  height: var(--f7-fab-button-size);
  margin-top: calc(-1 * var(--f7-fab-button-size) / 2);
}
.fab-buttons-left {
  right: 100%;
  margin-right: 16px;
  flex-direction: row-reverse;
}
.fab-buttons-left a {
  transform: translate3d(8px, 0px, 0) scale(0.3);
  transform-origin: right center;
}
.fab-buttons-left a + a {
  margin-right: 16px;
}
.fab-buttons-right {
  left: 100%;
  margin-left: 16px;
}
.fab-buttons-right a {
  transform: translate3d(-8px, 0, 0) scale(0.3);
  transform-origin: left center;
}
.fab-buttons-right a + a {
  margin-left: 16px;
}
.fab-buttons-center {
  left: 0%;
  top: 0%;
  width: 100%;
  height: 100%;
}
.fab-buttons-center a {
  position: absolute;
}
.fab-buttons-center a:nth-child(1) {
  left: 50%;
  margin-left: calc(-1 * var(--f7-fab-button-size) / 2);
  bottom: 100%;
  margin-bottom: 16px;
  transform: translateY(-8px) scale(0.3);
  transform-origin: center bottom;
}
.fab-buttons-center a:nth-child(2) {
  left: 100%;
  margin-top: calc(-1 * var(--f7-fab-button-size) / 2);
  top: 50%;
  margin-left: 16px;
  transform: translateX(-8px) scale(0.3);
  transform-origin: left center;
}
.fab-buttons-center a:nth-child(3) {
  left: 50%;
  margin-left: calc(-1 * var(--f7-fab-button-size) / 2);
  top: 100%;
  margin-top: 16px;
  transform: translateY(8px) scale(0.3);
  transform-origin: center top;
}
.fab-buttons-center a:nth-child(4) {
  right: 100%;
  margin-top: calc(-1 * var(--f7-fab-button-size) / 2);
  top: 50%;
  margin-right: 16px;
  transform: translateX(8px) scale(0.3);
  transform-origin: right center;
}
.fab-morph {
  border-radius: calc(var(--f7-fab-size) / 2);
  background: var(--f7-fab-bg-color, var(--f7-theme-color));
  box-shadow: var(--f7-fab-box-shadow);
}
.fab-morph > a {
  box-shadow: none;
  background: none !important;
}
.fab-opened.fab-morph > a i {
  opacity: 0;
}
.fab-morph,
.fab-morph > a,
.fab-morph-target {
  transition-duration: 250ms;
}
.fab-morph-target:not(.fab-morph-target-visible) {
  display: none;
}
.fab-extended {
  width: auto;
  min-width: var(--f7-fab-extended-size);
}
.fab-extended > a {
  width: 100%;
  height: var(--f7-fab-extended-size);
}
.fab-extended > a i {
  left: calc(var(--f7-fab-extended-size) / 2);
}
.fab-extended i ~ .fab-text {
  padding-left: var(--f7-fab-extended-size);
}
.fab-extended > a {
  width: 100% !important;
}
.fab-text {
  box-sizing: border-box;
  font-size: var(--f7-fab-extended-text-font-size);
  padding: var(--f7-fab-extended-text-padding);
  font-weight: var(--f7-fab-extended-text-font-weight);
  letter-spacing: var(--f7-fab-extended-text-letter-spacing);
  text-transform: uppercase;
}
.fab-label-button {
  overflow: visible !important;
}
.fab-label {
  position: absolute;
  top: 50%;
  padding: var(--f7-fab-label-padding);
  border-radius: var(--f7-fab-label-border-radius);
  background: var(--f7-fab-label-bg-color);
  color: var(--f7-fab-label-text-color);
  box-shadow: var(--f7-fab-label-box-shadow);
  white-space: nowrap;
  transform: translateY(-50%);
  pointer-events: none;
  font-size: var(--f7-fab-label-font-size);
}
.fab[class*="fab-right-"] .fab-label {
  right: 100%;
  margin-right: 8px;
}
.fab[class*="fab-left-"] .fab-label {
  left: 100%;
  margin-left: 8px;
}
.navbar ~ * .fab[class*="-top"],
.navbar ~ .fab[class*="-top"],
.navbars ~ * .fab[class*="-top"],
.navbars ~ .fab[class*="-top"] {
  margin-top: calc(var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.toolbar-top ~ * .fab[class*="-top"],
.toolbar-top ~ .fab[class*="-top"],
.ios .toolbar-top-ios ~ * .fab[class*="-top"],
.ios .toolbar-top-ios ~ .fab[class*="-top"],
.md .toolbar-top-md ~ * .fab[class*="-top"],
.md .toolbar-top-md ~ .fab[class*="-top"] {
  margin-top: var(--f7-toolbar-height);
}
.toolbar-bottom ~ * .fab[class*="-bottom"],
.toolbar-bottom ~ .fab[class*="-bottom"],
.ios .toolbar-bottom-ios ~ * .fab[class*="-bottom"],
.ios .toolbar-bottom-ios ~ .fab[class*="-bottom"],
.md .toolbar-bottom-md ~ * .fab[class*="-bottom"],
.md .toolbar-bottom-md ~ .fab[class*="-bottom"] {
  margin-bottom: var(--f7-toolbar-height);
}
.tabbar-labels.toolbar-bottom ~ * .fab[class*="-bottom"],
.tabbar-labels.toolbar-bottom ~ .fab[class*="-bottom"],
.ios .tabbar-labels.toolbar-bottom-ios ~ * .fab[class*="-bottom"],
.ios .tabbar-labels.toolbar-bottom-ios ~ .fab[class*="-bottom"],
.md .tabbar-labels.toolbar-bottom-md ~ * .fab[class*="-bottom"],
.md .tabbar-labels.toolbar-bottom-md ~ .fab[class*="-bottom"] {
  margin-bottom: var(--f7-tabbar-labels-height);
}
.tabbar-labels.toolbar-top ~ * .fab[class*="-bottom"],
.tabbar-labels.toolbar-top ~ .fab[class*="-bottom"],
.ios .tabbar-labels.toolbar-top-ios ~ * .fab[class*="-bottom"],
.ios .tabbar-labels.toolbar-top-ios ~ .fab[class*="-bottom"],
.md .tabbar-labels.toolbar-top-md ~ * .fab[class*="-bottom"],
.md .tabbar-labels.toolbar-top-md ~ .fab[class*="-bottom"] {
  margin-top: var(--f7-tabbar-labels-height);
}
.messagebar ~ * .fab[class*="-bottom"],
.messagebar ~ .fab[class*="-bottom"] {
  margin-bottom: var(--f7-messagebar-height);
}
.navbar + .toolbar-top ~ * .fab[class*="-top"],
.ios .navbar + .toolbar-top-ios ~ * .fab[class*="-top"],
.md .navbar + .toolbar-top-ios ~ * .fab[class*="-top"],
.navbar + .toolbar-top ~ .fab[class*="-top"],
.ios .navbar + .toolbar-top-ios ~ .fab[class*="-top"],
.md .navbar + .toolbar-top-ios ~ .fab[class*="-top"] {
  margin-top: calc(var(--f7-toolbar-height) + var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbar + .toolbar-top.tabbar-labels ~ * .fab[class*="-top"],
.ios .navbar + .toolbar-top-ios.tabbar-labels ~ * .fab[class*="-top"],
.md .navbar + .toolbar-top-ios.tabbar-labels ~ * .fab[class*="-top"],
.navbar + .toolbar-top.tabbar-labels ~ .fab[class*="-top"],
.ios .navbar + .toolbar-top-ios.tabbar-labels ~ .fab[class*="-top"],
.md .navbar + .toolbar-top-ios.tabbar-labels ~ .fab[class*="-top"] {
  margin-top: calc(var(--f7-tabbar-labels-height) + var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbars + .toolbar-top ~ * .fab[class*="-top"],
.ios .navbars + .toolbar-top-ios ~ * .fab[class*="-top"],
.navbars + .toolbar-top ~ .fab[class*="-top"],
.ios .navbars + .toolbar-top-ios ~ .fab[class*="-top"] {
  margin-top: calc(var(--f7-toolbar-height) + var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbars + .toolbar-top.tabbar-labels ~ * .fab[class*="-top"],
.ios .navbars + .toolbar-top-ios.tabbar-labels ~ * .fab[class*="-top"],
.navbars + .toolbar-top.tabbar-labels ~ .fab[class*="-top"],
.ios .navbars + .toolbar-top-ios.tabbar-labels ~ .fab[class*="-top"] {
  margin-top: calc(var(--f7-tabbar-labels-height) + var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.ios .fab > a.active-state,
.ios .fab-buttons a.active-state {
  transition-duration: 0ms;
}
/* === Searchbar === */
:root {
  /*
  --f7-searchbar-link-color: var(--f7-bars-link-color);
  --f7-searchbar-inline-input-font-size: var(--f7-searchbar-input-font-size);
  --f7-searchbar-inline-input-height: var(--f7-searchbar-input-height);
  */
  --f7-searchbar-input-border-width: 0px;
  --f7-searchbar-input-border-color: transparent;
  --f7-searchbar-input-text-color: #000;
  --f7-searchbar-placeholder-color: rgba(0, 0, 0, 0.4);
}
:root .theme-dark,
:root.theme-dark {
  --f7-searchbar-input-text-color: #fff;
  --f7-searchbar-placeholder-color: rgba(255, 255, 255, 0.4);
}
.ios {
  /*
  --f7-searchbar-bg-image: var(--f7-bars-bg-image);
  --f7-searchbar-bg-color: var(--f7-bars-bg-color);
  --f7-searchbar-bg-color-rgb: var(--f7-bars-bg-color-rgb);
  --f7-searchbar-border-color: var(--f7-bars-border-color);
  */
  --f7-searchbar-height: 44px;
  --f7-searchbar-inner-padding-left: 8px;
  --f7-searchbar-inner-padding-right: 8px;
  /*
  --f7-searchbar-link-color: var(--f7-bars-link-color, var(--f7-theme-color));
  */
  --f7-searchbar-input-font-size: 17px;
  --f7-searchbar-input-border-radius: 8px;
  --f7-searchbar-input-height: 32px;
  --f7-searchbar-input-padding-horizontal: 28px;
  /*
  --f7-searchbar-inline-input-padding-horizontal: var(--f7-searchbar-input-padding-horizontal);
  --f7-searchbar-input-clear-button-color: var(--f7-input-clear-button-color);
  */
  --f7-searchbar-backdrop-bg-color: rgba(0, 0, 0, 0.4);
  --f7-searchbar-shadow-image: none;
  --f7-searchbar-in-page-content-margin: 0px;
  --f7-searchbar-in-page-content-box-shadow: none;
  --f7-searchbar-in-page-content-border-radius: 0;
  --f7-searchbar-in-page-content-input-border-radius: 0;
  --f7-searchbar-search-icon-color: rgba(0, 0, 0, 0.4);
  --f7-searchbar-input-bg-color: #e4e4e4;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-searchbar-search-icon-color: rgba(255, 255, 255, 0.4);
  --f7-searchbar-input-bg-color: #2a2a2a;
}
.md {
  --f7-searchbar-border-color: transparent;
  --f7-searchbar-height: 48px;
  --f7-searchbar-inner-padding-left: 0px;
  --f7-searchbar-inner-padding-right: 0px;
  --f7-searchbar-link-color: #737373;
  --f7-searchbar-search-icon-color: #737373;
  --f7-searchbar-input-font-size: 20px;
  --f7-searchbar-input-border-radius: 0px;
  --f7-searchbar-input-height: 100%;
  --f7-searchbar-input-padding-horizontal: 48px;
  --f7-searchbar-inline-input-padding-horizontal: 24px;
  --f7-searchbar-input-clear-button-color: #737373;
  --f7-searchbar-backdrop-bg-color: rgba(0, 0, 0, 0.25);
  --f7-searchbar-shadow-image: var(--f7-bars-shadow-bottom-image);
  --f7-searchbar-in-page-content-margin: 8px;
  --f7-searchbar-in-page-content-box-shadow: var(--f7-elevation-1);
  --f7-searchbar-in-page-content-border-radius: 4px;
  --f7-searchbar-in-page-content-input-border-radius: 4px;
  --f7-searchbar-bg-color: #fff;
  --f7-searchbar-input-bg-color: #fff;
}
.md .theme-dark,
.md.theme-dark {
  --f7-searchbar-bg-color: #202020;
  --f7-searchbar-input-bg-color: #202020;
}
.aurora {
  /*
  --f7-searchbar-bg-image: var(--f7-bars-bg-image);
  --f7-searchbar-bg-color: var(--f7-bars-bg-color);
  --f7-searchbar-border-color: var(--f7-bars-border-color);
  */
  --f7-searchbar-height: 38px;
  --f7-searchbar-inner-padding-left: 8px;
  --f7-searchbar-inner-padding-right: 8px;
  /*
  --f7-searchbar-link-color: var(--f7-bars-link-color, var(--f7-theme-color));
  */
  --f7-searchbar-input-font-size: 13px;
  --f7-searchbar-input-border-radius: 4px;
  --f7-searchbar-input-height: 24px;
  --f7-searchbar-input-padding-horizontal: 24px;
  /*
  --f7-searchbar-inline-input-padding-horizontal: var(--f7-searchbar-input-padding-horizontal;
  --f7-searchbar-input-clear-button-color: var(--f7-input-clear-button-color);
  */
  --f7-searchbar-backdrop-bg-color: rgba(0, 0, 0, 0.4);
  --f7-searchbar-shadow-image: none;
  --f7-searchbar-in-page-content-margin: 0px;
  --f7-searchbar-in-page-content-box-shadow: none;
  --f7-searchbar-in-page-content-border-radius: 0;
  /*
  --f7-searchbar-in-page-content-input-border-radius: var(--f7-searchbar-input-border-radius);
  */
  --f7-searchbar-search-icon-color: rgba(0, 0, 0, 0.4);
  --f7-searchbar-input-bg-color: #fff;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-searchbar-input-bg-color: #333;
  --f7-searchbar-search-icon-color: rgba(255, 255, 255, 0.4);
}
.searchbar {
  width: 100%;
  position: relative;
  z-index: 200;
  height: var(--f7-searchbar-height);
  background-image: var(--f7-searchbar-bg-image, var(--f7-bars-bg-image));
  background-color: var(--f7-searchbar-bg-color, var(--f7-bars-bg-color));
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .searchbar {
    background-color: rgba(var(--f7-searchbar-bg-color-rgb, var(--f7-bars-bg-color-rgb)), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.ios .subnavbar .searchbar {
  background-color: transparent;
  -webkit-backdrop-filter: none;
          backdrop-filter: none;
}
.ios .subnavbar .searchbar:after {
  display: none !important;
}
.searchbar.no-hairline:after,
.searchbar.no-border:after {
  display: none !important;
}
.searchbar.no-shadow:before {
  display: none !important;
}
.searchbar:after {
  content: '';
  position: absolute;
  background-color: var(--f7-searchbar-border-color, var(--f7-bars-border-color));
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.page > .searchbar:not(.searchbar-inline) {
  z-index: 600;
}
.page > .searchbar:not(.searchbar-inline):before {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  top: 100%;
  bottom: auto;
  height: 8px;
  pointer-events: none;
  background: var(--f7-searchbar-shadow-image);
}
.searchbar input[type="text"],
.searchbar input[type="search"] {
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  display: block;
  border: var(--f7-searchbar-input-border-width) solid var(--f7-searchbar-input-border-color);
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  font-family: inherit;
  font-weight: normal;
  color: var(--f7-searchbar-input-text-color);
  font-size: var(--f7-searchbar-input-font-size);
  background-color: var(--f7-searchbar-input-bg-color);
  border-radius: var(--f7-searchbar-input-border-radius);
  position: relative;
  padding: 0;
  padding-left: calc(var(--f7-searchbar-input-padding-horizontal) + var(--f7-searchbar-input-extra-padding-left, 0px));
  padding-right: calc(var(--f7-searchbar-input-padding-horizontal) + var(--f7-searchbar-input-extra-padding-right, 0px));
}
.searchbar input[type="text"]::-webkit-input-placeholder,
.searchbar input[type="search"]::-webkit-input-placeholder {
  color: var(--f7-searchbar-placeholder-color);
  opacity: 1;
}
.searchbar input[type="text"]::-moz-placeholder,
.searchbar input[type="search"]::-moz-placeholder {
  color: var(--f7-searchbar-placeholder-color);
  opacity: 1;
}
.searchbar input[type="text"]::placeholder,
.searchbar input[type="search"]::placeholder {
  color: var(--f7-searchbar-placeholder-color);
  opacity: 1;
}
.searchbar input::-webkit-search-cancel-button {
  -webkit-appearance: none;
          appearance: none;
}
.searchbar .searchbar-input-wrap {
  flex-shrink: 1;
  width: 100%;
  height: var(--f7-searchbar-input-height);
  position: relative;
}
.searchbar a {
  color: var(--f7-searchbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.page > .searchbar:not(.searchbar-inline) {
  position: absolute;
  left: 0;
  top: 0;
}
.page-content .searchbar:not(.searchbar-inline) {
  border-radius: var(--f7-searchbar-in-page-content-border-radius);
  margin: var(--f7-searchbar-in-page-content-margin);
  width: auto;
  box-shadow: var(--f7-searchbar-in-page-content-box-shadow);
}
.page-content .searchbar:not(.searchbar-inline) .searchbar-inner,
.page-content .searchbar:not(.searchbar-inline) input[type="text"],
.page-content .searchbar:not(.searchbar-inline) input[type="search"] {
  border-radius: var(--f7-searchbar-in-page-content-input-border-radius, var(--f7-searchbar-input-border-radius));
}
.searchbar .input-clear-button {
  color: var(--f7-searchbar-input-clear-button-color, var(--f7-input-clear-button-color));
}
.searchbar-expandable {
  --f7-searchbar-expandable-size: var(--f7-searchbar-height);
  position: absolute;
  transition-duration: 300ms;
  pointer-events: none;
}
.navbar .searchbar-expandable {
  background: transparent;
}
.navbar .searchbar-expandable:after {
  display: none !important;
}
.navbar .searchbar.searchbar-expandable {
  --f7-searchbar-expandable-size: var(--f7-navbar-height);
}
.toolbar .searchbar.searchbar-expandable {
  --f7-searchbar-expandable-size: var(--f7-toolbar-height);
}
.subnavbar .searchbar.searchbar-expandable {
  --f7-searchbar-expandable-size: var(--f7-subnavbar-height);
}
.tabbar-labels .searchbar.searchbar-expandable {
  --f7-searchbar-expandable-size: var(--f7-tabbar-labels-height);
}
.searchbar-inner {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  box-sizing: border-box;
  padding: 0 calc(var(--f7-searchbar-inner-padding-right) + var(--f7-safe-area-right)) 0 calc(var(--f7-searchbar-inner-padding-left) + var(--f7-safe-area-left));
}
.searchbar-disable-button {
  cursor: pointer;
  pointer-events: none;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  background: none;
  border: none;
  outline: 0;
  padding: 0;
  margin: 0;
  width: auto;
  opacity: 0;
}
.searchbar-icon {
  pointer-events: none;
  background-position: center;
  background-repeat: no-repeat;
}
.searchbar-icon:after {
  color: var(--f7-searchbar-search-icon-color);
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
}
.searchbar-backdrop {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: 100;
  opacity: 0;
  pointer-events: none;
  transition-duration: 300ms;
  transform: translate3d(0, 0, 0);
  background: var(--f7-searchbar-backdrop-bg-color);
}
.searchbar-backdrop.searchbar-backdrop-in {
  opacity: 1;
  pointer-events: auto;
}
.page-content > .searchbar-backdrop {
  position: fixed;
}
.searchbar-not-found {
  display: none;
}
.hidden-by-searchbar,
.list .hidden-by-searchbar,
.list.li.hidden-by-searchbar,
.list li.hidden-by-searchbar {
  display: none !important;
}
.navbar.with-searchbar-expandable-enabled-no-transition,
.navbar.with-searchbar-expandable-enabled-no-transition {
  --f7-navbar-large-collapse-progress: 1;
}
.navbar.with-searchbar-expandable-enabled,
.navbar.with-searchbar-expandable-enabled {
  --f7-navbar-large-collapse-progress: 1;
}
.navbar.with-searchbar-expandable-enabled .navbar-bg,
.navbar.with-searchbar-expandable-enabled .navbar-bg,
.navbar.with-searchbar-expandable-enabled .title-large,
.navbar.with-searchbar-expandable-enabled .title-large,
.navbar.with-searchbar-expandable-enabled .title-large-text,
.navbar.with-searchbar-expandable-enabled .title-large-text {
  transition-duration: 300ms;
}
.navbar.with-searchbar-expandable-closing .navbar-bg,
.navbar.with-searchbar-expandable-closing .navbar-bg,
.navbar.with-searchbar-expandable-closing .title-large,
.navbar.with-searchbar-expandable-closing .title-large,
.navbar.with-searchbar-expandable-closing .title-large-text,
.navbar.with-searchbar-expandable-closing .title-large-text {
  transition-duration: 300ms;
}
.page-content.with-searchbar-expandable-enabled {
  height: calc(100% + var(--f7-navbar-large-title-height));
  transform: translateY(calc(-1 * var(--f7-navbar-large-title-height)));
  transition-duration: 300ms;
  transition-property: transform;
}
.page-content.with-searchbar-expandable-closing {
  transition-duration: 300ms;
}
.navbar ~ .page:not(.no-navbar) > .searchbar,
.navbars ~ .page:not(.no-navbar) > .searchbar,
.page > .navbar ~ .searchbar {
  top: calc(var(--f7-navbar-height) + var(--f7-safe-area-top));
}
.navbar ~ .page-with-navbar-large:not(.no-navbar) .searchbar,
.navbars ~ .page-with-navbar-large:not(.no-navbar) .searchbar,
.page-with-navbar-large .navbar ~ .searchbar,
.page-with-navbar-large .navbar ~ * .searchbar {
  top: calc(var(--f7-navbar-height) + var(--f7-navbar-large-title-height) + var(--f7-safe-area-top));
  transform: translate3d(0, calc(-1 * var(--f7-navbar-large-collapse-progress) * var(--f7-navbar-large-title-height)), 0);
}
.searchbar ~ * {
  --f7-page-searchbar-offset: var(--f7-searchbar-height);
}
.page > .toolbar-top ~ .searchbar,
.ios .page > .toolbar-top-ios ~ .searchbar,
.md .page > .toolbar-top-md ~ .searchbar,
.aurora .page > .toolbar-top-aurora ~ .searchbar {
  top: var(--f7-toolbar-height);
}
.page > .tabbar-labels.toolbar-top ~ .searchbar,
.ios .page > .tabbar-labels.toolbar-top-ios ~ .searchbar,
.md .page > .tabbar-labels.toolbar-top-md ~ .searchbar,
.aurora .page > .tabbar-labels.toolbar-top-aurora ~ .searchbar {
  top: var(--f7-tabbar-labels-height);
}
.page > .navbar ~ .toolbar-top ~ .searchbar,
.ios .page > .navbar ~ .toolbar-top-ios ~ .searchbar,
.md .page > .navbar ~ .toolbar-top-md ~ .searchbar,
.aurora .page > .navbar ~ .toolbar-top-aurora ~ .searchbar {
  top: calc(var(--f7-navbar-height) + var(--f7-toolbar-height) + var(--f7-safe-area-top));
}
.page > .navbar ~ .tabbar-labels.toolbar-top ~ .searchbar,
.ios .page > .navbar ~ .tabbar-labels.toolbar-top-ios ~ .searchbar,
.md .page > .navbar ~ .tabbar-labels.toolbar-top-md ~ .searchbar,
.aurora .page > .navbar ~ .tabbar-labels.toolbar-top-aurora ~ .searchbar {
  top: calc(var(--f7-navbar-height) + var(--f7-tabbar-labels-height) + var(--f7-safe-area-top));
}
.searchbar.searchbar-inline {
  width: auto;
  height: auto;
  background-color: transparent;
  background-image: none;
}
.searchbar.searchbar-inline:after,
.searchbar.searchbar-inline:before {
  display: none !important;
}
.searchbar.searchbar-inline .searchbar-input-wrap {
  height: var(--f7-searchbar-inline-input-height, var(--f7-searchbar-input-height));
}
.searchbar.searchbar-inline .searchbar-inner {
  padding: 0;
  position: static;
  width: auto;
  height: auto;
}
.searchbar.searchbar-inline input[type="text"],
.searchbar.searchbar-inline input[type="search"] {
  font-size: var(--f7-searchbar-inline-input-font-size, var(--f7-searchbar-input-font-size));
  padding-left: calc(var(--f7-searchbar-inline-input-padding-horizontal, var(--f7-searchbar-input-padding-horizontal)) + var(--f7-searchbar-input-extra-padding-left, 0px));
  padding-right: calc(var(--f7-searchbar-inline-input-padding-horizontal, var(--f7-searchbar-input-padding-horizontal)) + var(--f7-searchbar-input-extra-padding-right, 0px));
}
.ios .searchbar input[type="search"],
.ios .searchbar input[type="text"] {
  z-index: 30;
}
.ios .searchbar .input-clear-button {
  z-index: 40;
  right: 7px;
}
.ios .searchbar-icon {
  width: 13px;
  height: 13px;
  position: absolute;
  top: 50%;
  margin-top: -6px;
  z-index: 40;
  left: 8px;
}
.ios .searchbar-icon:after {
  content: 'search_ios';
  line-height: 13px;
}
.ios .searchbar-disable-button {
  font-size: 17px;
  flex-shrink: 0;
  transform: translate3d(0, 0, 0);
  transition-duration: 300ms;
  color: var(--f7-searchbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
  display: none;
}
.ios .searchbar-disable-button.active-state {
  transition-duration: 0ms;
  opacity: 0.3 !important;
}
.ios .searchbar-enabled .searchbar-disable-button {
  pointer-events: auto;
  opacity: 1;
  margin-left: 8px;
}
.ios .searchbar:not(.searchbar-enabled) .searchbar-disable-button {
  transition-duration: 300ms !important;
}
.ios .searchbar-expandable {
  left: 0;
  bottom: 0;
  opacity: 1;
  width: 100%;
  height: 0%;
  transform: translate3d(0, 0, 0);
  overflow: hidden;
}
.ios .searchbar-expandable .searchbar-disable-button {
  margin-left: 8px;
  opacity: 1;
  display: block;
}
.ios .searchbar-expandable .searchbar-inner {
  height: var(--f7-searchbar-expandable-size);
}
.ios .navbar.with-searchbar-expandable-enabled .navbar-bg,
.ios .navbar.with-searchbar-expandable-closing .navbar-bg {
  transition-property: transform, opacity;
}
.ios .navbar.with-searchbar-expandable-enabled .navbar-bg,
.ios .navbar.with-searchbar-expandable-closing .navbar-bg,
.ios .navbar.with-searchbar-expandable-enabled .left,
.ios .navbar.with-searchbar-expandable-closing .left,
.ios .navbar.with-searchbar-expandable-enabled .title,
.ios .navbar.with-searchbar-expandable-closing .title,
.ios .navbar.with-searchbar-expandable-enabled .right,
.ios .navbar.with-searchbar-expandable-closing .right {
  transition-duration: 300ms;
}
.ios .navbar.with-searchbar-expandable-enabled .left,
.ios .navbar.with-searchbar-expandable-enabled-no-transition .left,
.ios .navbar.with-searchbar-expandable-enabled .title,
.ios .navbar.with-searchbar-expandable-enabled-no-transition .title,
.ios .navbar.with-searchbar-expandable-enabled .right,
.ios .navbar.with-searchbar-expandable-enabled-no-transition .right {
  transform: translateY(calc(-1 * var(--f7-navbar-height)));
  opacity: 0 !important;
}
.ios .searchbar-expandable.searchbar-enabled {
  opacity: 1;
  height: var(--f7-searchbar-expandable-size);
  pointer-events: auto;
}
.md .searchbar-icon,
.md .searchbar-disable-button {
  position: absolute;
  left: calc(-4px + var(--f7-safe-area-left));
  top: 50%;
  transition-duration: 300ms;
}
.md .searchbar-icon {
  width: 24px;
  height: 24px;
  margin-left: 12px;
  margin-top: -12px;
}
.md .searchbar-icon:after {
  content: 'search_md';
  line-height: 1.2;
}
.md .searchbar-disable-button {
  width: 48px;
  height: 48px;
  transform: rotate(-90deg) scale(0.5);
  font-size: 0 !important;
  display: block;
  margin-top: -24px;
  color: var(--f7-searchbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.md .searchbar-disable-button:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .searchbar-disable-button.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .searchbar-disable-button:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  text-align: center;
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  line-height: 48px;
  content: "arrow_left_md";
}
.md .searchbar-enabled:not(.searchbar-enabled-no-disable-button) .searchbar-disable-button {
  transform: rotate(0deg) scale(1);
  pointer-events: auto;
  opacity: 1;
}
.md .searchbar-enabled:not(.searchbar-enabled-no-disable-button) .searchbar-icon {
  opacity: 0;
  transform: rotate(90deg) scale(0.5);
}
.md .searchbar {
  --f7-searchbar-input-extra-padding-left: 17px;
}
.md .searchbar .input-clear-button {
  width: 48px;
  height: 48px;
  margin-top: -24px;
  right: 0;
}
.md .searchbar .input-clear-button:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .searchbar .input-clear-button.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .searchbar .input-clear-button:after {
  line-height: 48px;
  content: 'delete_md';
  opacity: 1;
}
.md .searchbar .input-clear-button:before {
  margin-left: 0;
  margin-top: 0;
}
.md .page > .searchbar,
.md .subnavbar .searchbar,
.md .searchbar-expandable {
  --f7-searchbar-input-extra-padding-left: calc(17px + 8px);
}
.md .page > .searchbar .searchbar-icon,
.md .subnavbar .searchbar .searchbar-icon,
.md .searchbar-expandable .searchbar-icon,
.md .page > .searchbar .searchbar-disable-button,
.md .subnavbar .searchbar .searchbar-disable-button,
.md .searchbar-expandable .searchbar-disable-button {
  left: calc(-4px + 8px + var(--f7-safe-area-left));
}
.md .searchbar-expandable {
  height: var(--f7-searchbar-expandable-size);
  opacity: 0;
  bottom: 0;
  border-radius: calc(var(--f7-searchbar-expandable-size));
  width: calc(var(--f7-searchbar-expandable-size));
  margin-top: calc(var(--f7-searchbar-expandable-size) * -1 / 2);
  transform: translate3d(0px, 0px, 0px);
  left: 100%;
  margin-left: calc(var(--f7-searchbar-expandable-size) * -1);
}
.md .searchbar-expandable.searchbar-enabled {
  width: 100%;
  border-radius: 0;
  opacity: 1;
  pointer-events: auto;
  margin-top: 0;
  left: 0;
  margin-left: 0;
}
.aurora .searchbar input[type="search"],
.aurora .searchbar input[type="text"] {
  z-index: 30;
}
.aurora .searchbar .input-clear-button {
  z-index: 40;
  right: 4px;
}
.aurora .searchbar-icon {
  width: 13px;
  height: 13px;
  position: absolute;
  top: 50%;
  margin-top: -6px;
  z-index: 40;
  left: 6px;
}
.aurora .searchbar-icon:after {
  content: 'search_aurora';
  line-height: 13px;
}
.aurora .searchbar-disable-button {
  font-size: 14px;
  flex-shrink: 0;
  transform: translate3d(0, 0, 0);
  transition-duration: 300ms;
  color: var(--f7-searchbar-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
  display: none;
}
.aurora .searchbar-disable-button.active-state {
  transition-duration: 0ms;
  opacity: 0.3 !important;
}
.aurora .searchbar-enabled .searchbar-disable-button {
  pointer-events: auto;
  opacity: 1;
  margin-left: 8px;
}
.aurora .searchbar:not(.searchbar-enabled) .searchbar-disable-button {
  transition-duration: 300ms !important;
}
.aurora .searchbar-expandable {
  left: 0;
  top: auto;
  bottom: 0;
  opacity: 0;
  width: 100%;
  transform: translate3d(0, 0%, 0);
  overflow: hidden;
}
.aurora .searchbar-expandable .searchbar-disable-button {
  margin-left: 8px;
  opacity: 1;
  display: block;
}
.aurora .searchbar-expandable .searchbar-inner {
  height: var(--f7-searchbar-expandable-size);
}
.aurora .searchbar-expandable.searchbar-enabled {
  opacity: 1;
  pointer-events: auto;
}
/* === Messages === */
:root {
  --f7-message-text-header-text-color: inherit;
  --f7-message-text-header-opacity: 0.65;
  --f7-message-text-header-font-size: 12px;
  --f7-message-text-footer-text-color: inherit;
  --f7-message-text-footer-opacity: 0.65;
  --f7-message-text-footer-font-size: 12px;
  --f7-message-bubble-line-height: 1.2;
  --f7-message-header-font-size: 12px;
  --f7-message-footer-font-size: 11px;
  --f7-message-name-font-size: 12px;
  --f7-message-name-font-weight: inherit;
  --f7-message-avatar-border-radius: 50%;
  --f7-messages-title-font-weight: inherit;
  /*
  --f7-message-sent-bg-color: var(--f7-theme-color);
  */
  --f7-message-sent-text-color: #fff;
  --f7-messages-content-bg-color: #fff;
  --f7-message-typing-indicator-bg-color: #000;
  --f7-message-received-bg-color: #e5e5ea;
  --f7-message-received-text-color: #000;
}
:root .theme-dark,
:root.theme-dark {
  --f7-messages-title-text-color: rgba(255, 255, 255, 0.54);
  --f7-message-header-text-color: rgba(255, 255, 255, 0.54);
  --f7-message-name-text-color: rgba(255, 255, 255, 0.54);
  --f7-message-footer-text-color: rgba(255, 255, 255, 0.54);
  --f7-messages-content-bg-color: transparent;
  --f7-message-received-bg-color: #252525;
  --f7-message-received-text-color: #fff;
  --f7-message-typing-indicator-bg-color: #fff;
}
.ios {
  --f7-messages-title-text-color: rgba(0, 0, 0, 0.45);
  --f7-messages-title-font-size: 11px;
  --f7-message-header-text-color: rgba(0, 0, 0, 0.45);
  --f7-message-footer-text-color: rgba(0, 0, 0, 0.45);
  --f7-message-name-text-color: rgba(0, 0, 0, 0.45);
  --f7-message-avatar-size: 29px;
  --f7-message-margin: 10px;
  --f7-message-bubble-min-height: 32px;
  --f7-message-bubble-font-size: 17px;
  --f7-message-bubble-border-radius: 16px;
  --f7-message-bubble-padding-vertical: 6px;
  --f7-message-bubble-padding-horizontal: 16px;
  --f7-message-typing-indicator-opacity: 0.35;
}
.md {
  --f7-messages-title-font-size: 12px;
  --f7-message-avatar-size: 32px;
  --f7-message-margin: 16px;
  --f7-message-bubble-min-height: 32px;
  --f7-message-bubble-font-size: 16px;
  --f7-message-bubble-border-radius: 4px;
  --f7-message-bubble-padding-vertical: 6px;
  --f7-message-bubble-padding-horizontal: 8px;
  --f7-message-typing-indicator-opacity: 0.6;
  --f7-messages-title-text-color: rgba(0, 0, 0, 0.51);
  --f7-message-header-text-color: rgba(0, 0, 0, 0.51);
  --f7-message-footer-text-color: rgba(0, 0, 0, 0.51);
  --f7-message-name-text-color: rgba(0, 0, 0, 0.51);
}
.aurora {
  --f7-messages-title-font-size: 12px;
  --f7-message-avatar-size: 24px;
  --f7-message-margin: 10px;
  --f7-message-bubble-min-height: 28px;
  --f7-message-bubble-font-size: 13px;
  --f7-message-bubble-line-height: 1.4;
  --f7-message-bubble-border-radius: 14px;
  --f7-message-bubble-padding-vertical: 5px;
  --f7-message-bubble-padding-horizontal: 10px;
  --f7-message-typing-indicator-opacity: 0.5;
  --f7-messages-title-text-color: rgba(0, 0, 0, 0.51);
  --f7-message-header-text-color: rgba(0, 0, 0, 0.51);
  --f7-message-footer-text-color: rgba(0, 0, 0, 0.51);
  --f7-message-name-text-color: rgba(0, 0, 0, 0.51);
}
.messages-content,
.messages {
  background: var(--f7-messages-content-bg-color);
}
.messages {
  display: flex;
  flex-direction: column;
  min-height: 100%;
  position: relative;
  z-index: 1;
}
.messages-title,
.message {
  margin-top: var(--f7-message-margin);
}
.messages-title:last-child,
.message:last-child {
  margin-bottom: var(--f7-message-margin);
}
.messages-title {
  text-align: center;
  width: 100%;
  line-height: 1;
  color: var(--f7-messages-title-text-color);
  font-size: var(--f7-messages-title-font-size);
  font-weight: var(--f7-messages-title-font-weight);
}
.message {
  max-width: 70%;
  box-sizing: border-box;
  display: flex;
  align-items: flex-end;
  position: relative;
  z-index: 1;
  transform: translate3d(0, 0, 0);
}
.message-avatar {
  border-radius: var(--f7-message-avatar-border-radius);
  position: relative;
  background-size: cover;
  align-self: flex-end;
  flex-shrink: 0;
  width: var(--f7-message-avatar-size);
  height: var(--f7-message-avatar-size);
}
.message-content {
  position: relative;
  display: flex;
  flex-direction: column;
}
.message-header,
.message-footer,
.message-name {
  line-height: 1;
}
.message-header {
  color: var(--f7-message-header-text-color);
  font-size: var(--f7-message-header-font-size);
}
.message-footer {
  color: var(--f7-message-footer-text-color);
  font-size: var(--f7-message-footer-font-size);
  margin-bottom: -1em;
}
.message-name {
  color: var(--f7-message-name-text-color);
  font-size: var(--f7-message-name-font-size);
  font-weight: var(--f7-message-name-font-weight);
}
.message-bubble {
  box-sizing: border-box;
  word-break: break-word;
  display: flex;
  flex-direction: column;
  position: relative;
  line-height: var(--f7-message-bubble-line-height);
  font-size: var(--f7-message-bubble-font-size);
  border-radius: var(--f7-message-bubble-border-radius);
  padding: var(--f7-message-bubble-padding-vertical) var(--f7-message-bubble-padding-horizontal);
  min-height: var(--f7-message-bubble-min-height);
}
.message-image img {
  display: block;
  max-width: 100%;
  height: auto;
  width: auto;
}
.message-text-header,
.message-text-footer {
  line-height: 1;
}
.message-text-header {
  color: var(--f7-message-text-header-text-color);
  opacity: var(--f7-message-text-header-opacity);
  font-size: var(--f7-message-text-header-font-size);
}
.message-text-footer {
  color: var(--f7-message-text-footer-text-color);
  opacity: var(--f7-message-text-footer-opacity);
  font-size: var(--f7-message-text-footer-font-size);
}
.message-text {
  text-align: left;
}
.message-sent {
  text-align: right;
  flex-direction: row-reverse;
  align-self: flex-end;
}
.message-sent .message-bubble {
  color: var(--f7-message-sent-text-color);
  background: var(--f7-message-sent-bg-color, var(--f7-theme-color));
}
.message-sent .message-content {
  align-items: flex-end;
}
.message-sent.message-tail .message-bubble {
  border-radius: var(--f7-message-bubble-border-radius) var(--f7-message-bubble-border-radius) 0 var(--f7-message-bubble-border-radius);
}
.message-received {
  flex-direction: row;
}
.message-received .message-bubble {
  color: var(--f7-message-received-text-color);
  background: var(--f7-message-received-bg-color);
}
.message-received .message-content {
  align-items: flex-start;
}
.message-received.message-tail .message-bubble {
  border-radius: var(--f7-message-bubble-border-radius) var(--f7-message-bubble-border-radius) var(--f7-message-bubble-border-radius) 0;
}
.message:not(.message-last) .message-avatar {
  opacity: 0;
}
.message:not(.message-first) .message-name {
  display: none;
}
.message.message-same-name .message-name {
  display: none;
}
.message.message-same-header .message-header {
  display: none;
}
.message.message-same-footer .message-footer {
  display: none;
}
.message-appear-from-bottom {
  animation: message-appear-from-bottom 300ms;
}
.message-appear-from-top {
  animation: message-appear-from-top 300ms;
}
.message-typing-indicator {
  display: inline-block;
  font-size: 0;
  vertical-align: middle;
}
.message-typing-indicator > div {
  display: inline-block;
  position: relative;
  background: var(--f7-message-typing-indicator-bg-color);
  opacity: var(--f7-message-typing-indicator-opacity);
  vertical-align: middle;
  border-radius: 50%;
}
@keyframes message-appear-from-bottom {
  from {
    transform: translate3d(0, 100%, 0);
  }
  to {
    transform: translate3d(0, 0, 0);
  }
}
@keyframes message-appear-from-top {
  from {
    transform: translate3d(0, -100%, 0);
  }
  to {
    transform: translate3d(0, 0, 0);
  }
}
.ios .messages-title b,
.ios .message-header b,
.ios .message-footer b,
.ios .message-name b {
  font-weight: 600;
}
.ios .message-header,
.ios .message-name {
  margin-bottom: 3px;
}
.ios .message-footer {
  margin-top: 3px;
}
.ios .message-bubble {
  min-width: 48px;
}
.ios .message-image {
  margin: var(--f7-message-bubble-padding-vertical) calc(-1 * var(--f7-message-bubble-padding-horizontal));
}
.ios .message-image:first-child {
  margin-top: calc(-1 * var(--f7-message-bubble-padding-vertical));
}
.ios .message-image:first-child img {
  border-top-left-radius: var(--f7-message-bubble-border-radius);
  border-top-right-radius: var(--f7-message-bubble-border-radius);
}
.ios .message-image:last-child {
  margin-bottom: calc(-1 * var(--f7-message-bubble-padding-vertical));
}
.ios .message-image:last-child img {
  border-bottom-left-radius: var(--f7-message-bubble-border-radius);
  border-bottom-right-radius: var(--f7-message-bubble-border-radius);
}
.ios .message-text-header {
  margin-bottom: 3px;
}
.ios .message-text-footer {
  margin-top: 3px;
}
.ios .message-received {
  margin-left: calc(10px + var(--f7-safe-area-left));
}
.ios .message-received .message-header,
.ios .message-received .message-footer,
.ios .message-received .message-name {
  margin-left: var(--f7-message-bubble-padding-horizontal);
}
.ios .message-received .message-bubble {
  padding-left: calc(var(--f7-message-bubble-padding-horizontal) + 6px);
  -webkit-mask-box-image: url("data:image/svg+xml;charset=utf-8,<svg height='35' viewBox='0 0 96 70' width='48' xmlns='http://www.w3.org/2000/svg'><path d='m96 35c1 7-5 37-42 35-37 2-43-28-42-35-1-7 5-37 42-35 37-2 43 28 42 35z'/></svg>") 50% 42% 46% 56%;
}
.ios .message-received .message-image {
  margin-left: calc(-1 * (var(--f7-message-bubble-padding-horizontal) + 6px));
}
.ios .message-received.message-tail:not(.message-typing) .message-bubble {
  -webkit-mask-box-image: url("data:image/svg+xml;charset=utf-8,<svg height='35' viewBox='0 0 96 70' width='48' xmlns='http://www.w3.org/2000/svg'><path d='m96 35c1 7-5 37-42 35-37 2-43-28-42-35-1-7 5-37 42-35 37-2 43 28 42 35z'/><path d='m0 70c6-2 12-10 12-19v-16l14 27s-8 8-26 8z'/></svg>") 50% 42% 46% 56%;
}
.ios .message-received.message-tail:not(.message-typing) .message-bubble .message-image:last-child img {
  border-bottom-left-radius: 0px;
}
.ios .message-sent {
  margin-right: calc(10px + var(--f7-safe-area-right));
}
.ios .message-sent .message-header,
.ios .message-sent .message-footer,
.ios .message-sent .message-name {
  margin-right: var(--f7-message-bubble-padding-horizontal);
}
.ios .message-sent .message-bubble {
  padding-right: calc(var(--f7-message-bubble-padding-horizontal) + 6px);
  -webkit-mask-box-image: url("data:image/svg+xml;charset=utf-8,<svg height='35' viewBox='0 0 96 70' width='48' xmlns='http://www.w3.org/2000/svg'><path d='m84 35c1 7-5 37-42 35-37 2-43-28-42-35-1-7 5-37 42-35 37-2 43 28 42 35z'/></svg>") 50% 56% 46% 42%;
}
.ios .message-sent .message-image {
  margin-right: calc(-1 * (var(--f7-message-bubble-padding-horizontal) + 6px));
}
.ios .message-sent.message-tail .message-bubble {
  -webkit-mask-box-image: url("data:image/svg+xml;charset=utf-8,<svg height='35' viewBox='0 0 96 70' width='48' xmlns='http://www.w3.org/2000/svg'><path d='m84 35c1 7-5 37-42 35-37 2-43-28-42-35-1-7 5-37 42-35 37-2 43 28 42 35z'/><path d='m96 70c-6-2-12-10-12-19v-16l-14 27s8 8 26 8z'/></svg>") 50% 56% 46% 42%;
}
.ios .message-sent.message-tail .message-bubble .message-image:last-child img {
  border-bottom-right-radius: 0px;
}
.ios .message + .message:not(.message-first) {
  margin-top: 1px;
}
.ios .message-received.message-typing .message-content:after,
.ios .message-received.message-typing .message-content:before {
  content: '';
  position: absolute;
  background: var(--f7-message-received-bg-color);
  border-radius: 50%;
}
.ios .message-received.message-typing .message-content:after {
  width: 11px;
  height: 11px;
  left: 4px;
  bottom: 0px;
}
.ios .message-received.message-typing .message-content:before {
  width: 6px;
  height: 6px;
  left: -1px;
  bottom: -4px;
}
.ios .message-typing-indicator > div {
  width: 9px;
  height: 9px;
}
.ios .message-typing-indicator > div + div {
  margin-left: 4px;
}
.ios .message-typing-indicator > div:nth-child(1) {
  animation: ios-message-typing-indicator 900ms infinite;
}
.ios .message-typing-indicator > div:nth-child(2) {
  animation: ios-message-typing-indicator 900ms 150ms infinite;
}
.ios .message-typing-indicator > div:nth-child(3) {
  animation: ios-message-typing-indicator 900ms 300ms infinite;
}
@keyframes ios-message-typing-indicator {
  0% {
    opacity: 0.35;
  }
  25% {
    opacity: 0.2;
  }
  50% {
    opacity: 0.2;
  }
}
.md .messages-title b,
.md .message-header b,
.md .message-footer b,
.md .message-name b {
  font-weight: 500;
}
.md .message-header,
.md .message-name {
  margin-bottom: 2px;
}
.md .message-footer {
  margin-top: 2px;
}
.md .message-text-header {
  margin-bottom: 4px;
}
.md .message-text-footer {
  margin-top: 4px;
}
.md .message-received.message-tail .message-bubble:before,
.md .message-sent.message-tail .message-bubble:before {
  position: absolute;
  content: '';
  bottom: 0;
  width: 0;
  height: 0;
}
.md .message-received {
  margin-left: calc(8px + var(--f7-safe-area-left));
}
.md .message-received .message-avatar + .message-content {
  margin-left: var(--f7-message-bubble-padding-horizontal);
}
.md .message-received.message-tail .message-bubble:before {
  border-left: 8px solid transparent;
  border-right: 0 solid transparent;
  border-bottom: 8px solid var(--f7-message-received-bg-color);
  right: 100%;
}
.md .message-sent {
  margin-right: calc(8px + var(--f7-safe-area-right));
}
.md .message-sent .message-avatar + .message-content {
  margin-right: var(--f7-message-bubble-padding-horizontal);
}
.md .message-sent.message-tail .message-bubble:before {
  border-left: 0 solid transparent;
  border-right: 8px solid transparent;
  border-bottom: 8px solid var(--f7-message-sent-bg-color, var(--f7-theme-color));
  left: 100%;
}
.md .message + .message:not(.message-first) {
  margin-top: 8px;
}
.md .message-typing-indicator > div {
  width: 6px;
  height: 6px;
}
.md .message-typing-indicator > div + div {
  margin-left: 6px;
}
.md .message-typing-indicator > div:nth-child(1) {
  animation: md-message-typing-indicator 900ms infinite;
}
.md .message-typing-indicator > div:nth-child(2) {
  animation: md-message-typing-indicator 900ms 150ms infinite;
}
.md .message-typing-indicator > div:nth-child(3) {
  animation: md-message-typing-indicator 900ms 300ms infinite;
}
@keyframes md-message-typing-indicator {
  0% {
    transform: translateY(0%);
  }
  25% {
    transform: translateY(-5px);
  }
  50% {
    transform: translateY(0%);
  }
}
.aurora .messages-title b,
.aurora .message-header b,
.aurora .message-footer b,
.aurora .message-name b {
  font-weight: 500;
}
.aurora .message-header,
.aurora .message-name {
  margin-bottom: 2px;
}
.aurora .message-footer {
  margin-top: 2px;
}
.aurora .message-text-header {
  margin-bottom: 2px;
}
.aurora .message-text-footer {
  margin-top: 2px;
}
.aurora .message-received.message-tail .message-bubble:before,
.aurora .message-sent.message-tail .message-bubble:before {
  position: absolute;
  content: '';
  bottom: 0;
  width: 0;
  height: 0;
}
.aurora .message-image {
  margin: var(--f7-message-bubble-padding-vertical) calc(-1 * var(--f7-message-bubble-padding-horizontal) + 4px);
}
.aurora .message-image:first-child {
  margin-top: calc(-1 * var(--f7-message-bubble-padding-vertical) + 4px);
}
.aurora .message-image:first-child img {
  border-top-left-radius: var(--f7-message-bubble-border-radius);
  border-top-right-radius: var(--f7-message-bubble-border-radius);
}
.aurora .message-image:last-child {
  margin-bottom: calc(-1 * var(--f7-message-bubble-padding-vertical) + 4px);
}
.aurora .message-image:last-child img {
  border-bottom-left-radius: var(--f7-message-bubble-border-radius);
  border-bottom-right-radius: var(--f7-message-bubble-border-radius);
}
.aurora .message-received {
  margin-left: calc(16px + var(--f7-safe-area-left));
}
.aurora .message-received .message-avatar + .message-content {
  margin-left: 5px;
}
.aurora .message-received .message-header,
.aurora .message-received .message-footer,
.aurora .message-received .message-name {
  margin-left: var(--f7-message-bubble-padding-horizontal);
}
.aurora .message-received.message-tail .message-bubble:before {
  border-left: 6px solid transparent;
  border-right: 0 solid transparent;
  border-bottom: 6px solid var(--f7-message-received-bg-color);
  right: 100%;
  transform: translate(2px, 0px) rotate(-15deg);
  transform-origin: right bottom;
}
.aurora .message-sent {
  margin-right: calc(16px + var(--f7-safe-area-right));
}
.aurora .message-sent .message-avatar + .message-content {
  margin-right: 5px;
}
.aurora .message-sent .message-header,
.aurora .message-sent .message-footer,
.aurora .message-sent .message-name {
  margin-right: var(--f7-message-bubble-padding-horizontal);
}
.aurora .message-sent.message-tail .message-bubble:before {
  border-left: 0 solid transparent;
  border-right: 6px solid transparent;
  border-bottom: 6px solid var(--f7-message-sent-bg-color, var(--f7-theme-color));
  left: 100%;
  transform: translate(-2px, 0px) rotate(15deg);
  transform-origin: left bottom;
}
.aurora .message + .message:not(.message-first) {
  margin-top: 5px;
}
.aurora .message-typing-indicator > div {
  width: 6px;
  height: 6px;
}
.aurora .message-typing-indicator > div + div {
  margin-left: 4px;
}
.aurora .message-typing-indicator > div:nth-child(1) {
  animation: aurora-message-typing-indicator 900ms infinite;
}
.aurora .message-typing-indicator > div:nth-child(2) {
  animation: aurora-message-typing-indicator 900ms 150ms infinite;
}
.aurora .message-typing-indicator > div:nth-child(3) {
  animation: aurora-message-typing-indicator 900ms 300ms infinite;
}
@keyframes aurora-message-typing-indicator {
  0% {
    transform: translateY(0%);
  }
  50% {
    transform: translateY(-5px);
  }
  100% {
    transform: translateY(0%);
  }
}
/* === Messagebar === */
:root {
  --f7-messagebar-shadow-image: none;
  --f7-messagebar-textarea-bg-color: transparent;
  --f7-messagebar-attachments-height: 155px;
  --f7-messagebar-attachment-height: 155px;
  --f7-messagebar-attachment-landscape-height: 120px;
  --f7-messagebar-sheet-height: 252px;
  --f7-messagebar-sheet-landscape-height: 192px;
  /*
  --f7-messagebar-inner-padding-left: var(--f7-toolbar-inner-padding-left);
  --f7-messagebar-inner-padding-right: var(--f7-toolbar-inner-padding-right);
  */
  --f7-messagebar-bg-color: #fff;
  --f7-messagebar-bg-color-rgb: 255, 255, 255;
}
:root .theme-dark,
:root.theme-dark {
  --f7-messagebar-bg-color: var(--f7-bars-bg-color);
  --f7-messagebar-bg-color-rgb: var(--f7-bars-bg-color-rgb);
}
.ios {
  --f7-messagebar-height: 44px;
  --f7-messagebar-font-size: 17px;
  /*
  --f7-messagebar-link-color: var(--f7-theme-color);
  */
  --f7-messagebar-border-color: transparent;
  --f7-messagebar-textarea-border-radius: 17px;
  --f7-messagebar-textarea-padding: 6px 16px;
  --f7-messagebar-textarea-height: 34px;
  --f7-messagebar-textarea-font-size: 17px;
  --f7-messagebar-textarea-line-height: 20px;
  --f7-messagebar-sheet-bg-color: #d1d5da;
  --f7-messagebar-attachment-border-radius: 12px;
  --f7-messagebar-textarea-text-color: #000;
  --f7-messagebar-textarea-border: 1px solid #c8c8cd;
  --f7-messagebar-attachments-border-color: #c8c8cd;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-messagebar-textarea-text-color: #fff;
  --f7-messagebar-textarea-border: 1px solid var(--f7-bars-border-color);
  --f7-messagebar-attachments-border-color: var(--f7-bars-border-color);
}
.md {
  --f7-messagebar-height: 48px;
  --f7-messagebar-font-size: 16px;
  --f7-messagebar-textarea-border-radius: 0px;
  --f7-messagebar-textarea-padding: 5px 8px;
  --f7-messagebar-textarea-height: 32px;
  --f7-messagebar-textarea-font-size: 16px;
  --f7-messagebar-textarea-line-height: 22px;
  --f7-messagebar-textarea-border: 1px solid transparent;
  --f7-messagebar-sheet-bg-color: #fff;
  --f7-messagebar-attachment-border-radius: 4px;
  --f7-messagebar-link-color: #333;
  --f7-messagebar-border-color: #d1d1d1;
  --f7-messagebar-textarea-text-color: #333;
  --f7-messagebar-attachments-border-color: #ddd;
}
.md .theme-dark,
.md.theme-dark {
  --f7-messagebar-border-color: transparent;
  --f7-messagebar-link-color: rgba(255, 255, 255, 0.87);
  --f7-messagebar-textarea-text-color: rgba(255, 255, 255, 0.87);
  --f7-messagebar-attachments-border-color: rgba(255, 255, 255, 0.2);
}
.aurora {
  --f7-messagebar-height: 38px;
  --f7-messagebar-font-size: 14px;
  /*
  --f7-messagebar-link-color: var(--f7-theme-color);
  */
  --f7-messagebar-border-color: transparent;
  --f7-messagebar-textarea-border-radius: 12px;
  --f7-messagebar-textarea-padding: 3px 10px;
  --f7-messagebar-textarea-height: 24px;
  --f7-messagebar-textarea-font-size: 13px;
  --f7-messagebar-textarea-line-height: 16px;
  --f7-messagebar-sheet-bg-color: #fff;
  --f7-messagebar-attachment-border-radius: 12px;
  --f7-messagebar-textarea-text-color: #000;
  --f7-messagebar-textarea-border: 1px solid #c8c8cd;
  --f7-messagebar-attachments-border-color: #c8c8cd;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-messagebar-textarea-text-color: #fff;
  --f7-messagebar-textarea-border: 1px solid var(--f7-bars-border-color);
  --f7-messagebar-attachments-border-color: var(--f7-bars-border-color);
}
.messagebar {
  transform: translate3d(0, 0, 0);
  background: var(--f7-messagebar-bg-color);
  height: auto;
  min-height: var(--f7-messagebar-height);
  font-size: var(--f7-messagebar-font-size);
  padding-bottom: var(--f7-safe-area-bottom);
  bottom: 0;
}
.messagebar:before {
  content: '';
  position: absolute;
  background-color: var(--f7-messagebar-border-color);
  display: block;
  z-index: 15;
  top: 0;
  right: auto;
  bottom: auto;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 0%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
.messagebar:after {
  content: '';
  position: absolute;
  right: 0;
  width: 100%;
  bottom: 100%;
  height: 8px;
  top: auto;
  pointer-events: none;
  background: var(--f7-messagebar-shadow-image);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-bars .messagebar {
    background-color: rgba(var(--f7-messagebar-bg-color-rgb), var(--f7-bars-translucent-opacity));
    -webkit-backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
            backdrop-filter: saturate(180%) blur(var(--f7-bars-translucent-blur));
  }
}
.messagebar.no-hairline:before,
.messagebar.no-border:before {
  display: none !important;
}
.messagebar.no-shadow:after,
.messagebar.toolbar-hidden:after {
  display: none !important;
}
.messagebar .toolbar-inner {
  top: auto;
  position: relative;
  height: auto;
  bottom: auto;
  padding-left: calc(var(--f7-messagebar-inner-padding-left, var(--f7-toolbar-inner-padding-left)) + var(--f7-safe-area-left));
  padding-right: calc(var(--f7-messagebar-inner-padding-right, var(--f7-toolbar-inner-padding-right)) + var(--f7-safe-area-right));
}
.messagebar.messagebar-sheet-visible > .toolbar-inner {
  bottom: 0;
}
.messagebar .messagebar-area {
  width: 100%;
  flex-shrink: 1;
  overflow: hidden;
  position: relative;
}
.messagebar textarea {
  width: 100%;
  flex-shrink: 1;
  background-color: var(--f7-messagebar-textarea-bg-color);
  border-radius: var(--f7-messagebar-textarea-border-radius);
  padding: var(--f7-messagebar-textarea-padding);
  height: var(--f7-messagebar-textarea-height);
  color: var(--f7-messagebar-textarea-text-color);
  font-size: var(--f7-messagebar-textarea-font-size);
  line-height: var(--f7-messagebar-textarea-line-height);
  border: var(--f7-messagebar-textarea-border);
}
.messagebar a.link {
  align-self: flex-end;
  flex-shrink: 0;
  color: var(--f7-messagebar-link-color, var(--f7-theme-color));
}
.messagebar-attachments {
  width: 100%;
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  font-size: 0;
  white-space: nowrap;
  box-sizing: border-box;
  position: relative;
}
.messagebar:not(.messagebar-attachments-visible) .messagebar-attachments {
  display: none;
}
.messagebar-attachment {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  display: inline-block;
  vertical-align: middle;
  white-space: normal;
  height: var(--f7-messagebar-attachment-height);
  position: relative;
  border-radius: var(--f7-messagebar-attachment-border-radius);
}
@media (orientation: landscape) {
  .messagebar-attachment {
    height: var(--f7-messagebar-attachment-landscape-height);
  }
}
.messagebar-attachment img {
  display: block;
  width: auto;
  height: 100%;
  border-radius: var(--f7-messagebar-attachment-border-radius);
}
.messagebar-attachment + .messagebar-attachment {
  margin-left: 8px;
}
.messagebar-sheet {
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  align-content: flex-start;
  height: var(--f7-messagebar-sheet-height);
  background-color: var(--f7-messagebar-sheet-bg-color);
  padding-left: var(--f7-safe-area-left);
  padding-right: var(--f7-safe-area-right);
}
@media (orientation: landscape) {
  .messagebar-sheet {
    height: var(--f7-messagebar-sheet-landscape-height);
  }
}
.messagebar-sheet-image,
.messagebar-sheet-item {
  box-sizing: border-box;
  flex-shrink: 0;
  margin-top: 1px;
  position: relative;
  overflow: hidden;
  height: calc((var(--f7-messagebar-sheet-height) - 2px) / 2);
  width: calc((var(--f7-messagebar-sheet-height) - 2px) / 2);
  margin-left: 1px;
}
@media (orientation: landscape) {
  .messagebar-sheet-image,
  .messagebar-sheet-item {
    width: calc((var(--f7-messagebar-sheet-landscape-height) - 2px) / 2);
    height: calc((var(--f7-messagebar-sheet-landscape-height) - 2px) / 2);
  }
}
.messagebar-sheet-image .icon-checkbox,
.messagebar-sheet-item .icon-checkbox,
.messagebar-sheet-image .icon-radio,
.messagebar-sheet-item .icon-radio {
  position: absolute;
  right: 8px;
  bottom: 8px;
}
.messagebar-sheet-image {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.messagebar-attachment-delete {
  display: block;
  position: absolute;
  border-radius: 50%;
  box-sizing: border-box;
  cursor: pointer;
  box-shadow: 0px 0px 2px rgba(0, 0, 0, 0.2);
}
.messagebar-attachment-delete:after,
.messagebar-attachment-delete:before {
  position: absolute;
  content: '';
  left: 50%;
  top: 50%;
}
.messagebar-attachment-delete:after {
  transform: rotate(45deg);
}
.messagebar-attachment-delete:before {
  transform: rotate(-45deg);
}
.messagebar:not(.messagebar-sheet-visible) .messagebar-sheet {
  display: none;
}
.messagebar ~ * {
  --f7-page-toolbar-bottom-offset: var(--f7-messagebar-height);
}
.ios .messagebar a.link.icon-only:first-child {
  margin-left: -8px;
}
.ios .messagebar a.link.icon-only:last-child {
  margin-right: -8px;
}
.ios .messagebar a.link:not(.icon-only) + .messagebar-area {
  margin-left: 8px;
}
.ios .messagebar .messagebar-area + a.link:not(.icon-only) {
  margin-left: 8px;
}
.ios .messagebar-area {
  margin-top: 5px;
  margin-bottom: 5px;
}
.ios .messagebar-attachments {
  padding: 5px;
  border-radius: var(--f7-messagebar-textarea-border-radius) var(--f7-messagebar-textarea-border-radius) 0 0;
  border: 1px solid var(--f7-messagebar-attachments-border-color);
  border-bottom: none;
}
.ios .messagebar-attachments-visible .messagebar-attachments + textarea {
  border-radius: 0 0 var(--f7-messagebar-textarea-border-radius) var(--f7-messagebar-textarea-border-radius);
}
.ios .messagebar-attachment {
  font-size: 14px;
}
.ios .messagebar-attachment-delete {
  right: 5px;
  top: 5px;
  width: 20px;
  height: 20px;
  background: #7d7e80;
  border: 2px solid #fff;
}
.ios .messagebar-attachment-delete:after,
.ios .messagebar-attachment-delete:before {
  width: 10px;
  height: 2px;
  background: #fff;
  margin-left: -5px;
  margin-top: -1px;
}
.md .messagebar-attachments {
  padding: 8px;
  border-bottom: 1px solid var(--f7-messagebar-attachments-border-color);
}
.md .messagebar-area {
  margin-top: 8px;
  margin-bottom: 8px;
}
.md .messagebar-sheet-image .icon-checkbox,
.md .messagebar-sheet-item .icon-checkbox {
  border-color: #fff;
  background: rgba(255, 255, 255, 0.25);
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
}
.md .messagebar-attachment-delete {
  right: 8px;
  top: 8px;
  width: 24px;
  height: 24px;
  background-color: var(--f7-theme-color);
  border-radius: 4px;
}
.md .messagebar-attachment-delete:after,
.md .messagebar-attachment-delete:before {
  width: 14px;
  height: 2px;
  background: #fff;
  margin-left: -7px;
  margin-top: -1px;
}
.aurora .messagebar a.link + .messagebar-area {
  margin-left: 5px;
}
.aurora .messagebar .messagebar-area + a.link {
  margin-left: 5px;
}
.aurora .messagebar-area {
  margin-top: 5px;
  margin-bottom: 5px;
}
.aurora .messagebar-sheet-image .icon-checkbox,
.aurora .messagebar-sheet-item .icon-checkbox {
  background: rgba(255, 255, 255, 0.25);
}
.aurora .messagebar-attachments {
  padding: 5px;
  border-radius: var(--f7-messagebar-textarea-border-radius) var(--f7-messagebar-textarea-border-radius) 0 0;
  border: 1px solid var(--f7-messagebar-attachments-border-color);
  border-bottom: none;
}
.aurora .messagebar-attachments-visible .messagebar-attachments + textarea {
  border-radius: 0 0 var(--f7-messagebar-textarea-border-radius) var(--f7-messagebar-textarea-border-radius);
}
.aurora .messagebar-attachment {
  font-size: 14px;
}
.aurora .messagebar-attachment-delete {
  right: 5px;
  top: 5px;
  width: 14px;
  height: 14px;
  background: #808080;
}
.aurora .messagebar-attachment-delete:after,
.aurora .messagebar-attachment-delete:before {
  width: 8px;
  height: 1px;
  background: #fff;
  margin-left: -4px;
  margin-top: -1px;
}
/* === Swiper === */
@font-face {
  font-family: 'swiper-icons';
  src: url("data:application/font-woff;charset=utf-8;base64, d09GRgABAAAAAAZgABAAAAAADAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABGRlRNAAAGRAAAABoAAAAci6qHkUdERUYAAAWgAAAAIwAAACQAYABXR1BPUwAABhQAAAAuAAAANuAY7+xHU1VCAAAFxAAAAFAAAABm2fPczU9TLzIAAAHcAAAASgAAAGBP9V5RY21hcAAAAkQAAACIAAABYt6F0cBjdnQgAAACzAAAAAQAAAAEABEBRGdhc3AAAAWYAAAACAAAAAj//wADZ2x5ZgAAAywAAADMAAAD2MHtryVoZWFkAAABbAAAADAAAAA2E2+eoWhoZWEAAAGcAAAAHwAAACQC9gDzaG10eAAAAigAAAAZAAAArgJkABFsb2NhAAAC0AAAAFoAAABaFQAUGG1heHAAAAG8AAAAHwAAACAAcABAbmFtZQAAA/gAAAE5AAACXvFdBwlwb3N0AAAFNAAAAGIAAACE5s74hXjaY2BkYGAAYpf5Hu/j+W2+MnAzMYDAzaX6QjD6/4//Bxj5GA8AuRwMYGkAPywL13jaY2BkYGA88P8Agx4j+/8fQDYfA1AEBWgDAIB2BOoAeNpjYGRgYNBh4GdgYgABEMnIABJzYNADCQAACWgAsQB42mNgYfzCOIGBlYGB0YcxjYGBwR1Kf2WQZGhhYGBiYGVmgAFGBiQQkOaawtDAoMBQxXjg/wEGPcYDDA4wNUA2CCgwsAAAO4EL6gAAeNpj2M0gyAACqxgGNWBkZ2D4/wMA+xkDdgAAAHjaY2BgYGaAYBkGRgYQiAHyGMF8FgYHIM3DwMHABGQrMOgyWDLEM1T9/w8UBfEMgLzE////P/5//f/V/xv+r4eaAAeMbAxwIUYmIMHEgKYAYjUcsDAwsLKxc3BycfPw8jEQA/gZBASFhEVExcQlJKWkZWTl5BUUlZRVVNXUNTQZBgMAAMR+E+gAEQFEAAAAKgAqACoANAA+AEgAUgBcAGYAcAB6AIQAjgCYAKIArAC2AMAAygDUAN4A6ADyAPwBBgEQARoBJAEuATgBQgFMAVYBYAFqAXQBfgGIAZIBnAGmAbIBzgHsAAB42u2NMQ6CUAyGW568x9AneYYgm4MJbhKFaExIOAVX8ApewSt4Bic4AfeAid3VOBixDxfPYEza5O+Xfi04YADggiUIULCuEJK8VhO4bSvpdnktHI5QCYtdi2sl8ZnXaHlqUrNKzdKcT8cjlq+rwZSvIVczNiezsfnP/uznmfPFBNODM2K7MTQ45YEAZqGP81AmGGcF3iPqOop0r1SPTaTbVkfUe4HXj97wYE+yNwWYxwWu4v1ugWHgo3S1XdZEVqWM7ET0cfnLGxWfkgR42o2PvWrDMBSFj/IHLaF0zKjRgdiVMwScNRAoWUoH78Y2icB/yIY09An6AH2Bdu/UB+yxopYshQiEvnvu0dURgDt8QeC8PDw7Fpji3fEA4z/PEJ6YOB5hKh4dj3EvXhxPqH/SKUY3rJ7srZ4FZnh1PMAtPhwP6fl2PMJMPDgeQ4rY8YT6Gzao0eAEA409DuggmTnFnOcSCiEiLMgxCiTI6Cq5DZUd3Qmp10vO0LaLTd2cjN4fOumlc7lUYbSQcZFkutRG7g6JKZKy0RmdLY680CDnEJ+UMkpFFe1RN7nxdVpXrC4aTtnaurOnYercZg2YVmLN/d/gczfEimrE/fs/bOuq29Zmn8tloORaXgZgGa78yO9/cnXm2BpaGvq25Dv9S4E9+5SIc9PqupJKhYFSSl47+Qcr1mYNAAAAeNptw0cKwkAAAMDZJA8Q7OUJvkLsPfZ6zFVERPy8qHh2YER+3i/BP83vIBLLySsoKimrqKqpa2hp6+jq6RsYGhmbmJqZSy0sraxtbO3sHRydnEMU4uR6yx7JJXveP7WrDycAAAAAAAH//wACeNpjYGRgYOABYhkgZgJCZgZNBkYGLQZtIJsFLMYAAAw3ALgAeNolizEKgDAQBCchRbC2sFER0YD6qVQiBCv/H9ezGI6Z5XBAw8CBK/m5iQQVauVbXLnOrMZv2oLdKFa8Pjuru2hJzGabmOSLzNMzvutpB3N42mNgZGBg4GKQYzBhYMxJLMlj4GBgAYow/P/PAJJhLM6sSoWKfWCAAwDAjgbRAAB42mNgYGBkAIIbCZo5IPrmUn0hGA0AO8EFTQAA") format("woff");
  font-weight: 400;
  font-style: normal;
}
:root {
  --swiper-theme-color: #007aff;
}
.swiper-container {
  margin-left: auto;
  margin-right: auto;
  position: relative;
  overflow: hidden;
  list-style: none;
  padding: 0;
  /* Fix of Webkit flickering */
  z-index: 1;
}
.swiper-container-vertical > .swiper-wrapper {
  flex-direction: column;
}
.swiper-wrapper {
  position: relative;
  width: 100%;
  height: 100%;
  z-index: 1;
  display: flex;
  transition-property: transform;
  box-sizing: content-box;
}
.swiper-container-android .swiper-slide,
.swiper-wrapper {
  transform: translate3d(0px, 0, 0);
}
.swiper-container-multirow > .swiper-wrapper {
  flex-wrap: wrap;
}
.swiper-container-multirow-column > .swiper-wrapper {
  flex-wrap: wrap;
  flex-direction: column;
}
.swiper-container-free-mode > .swiper-wrapper {
  transition-timing-function: ease-out;
  margin: 0 auto;
}
.swiper-slide {
  flex-shrink: 0;
  width: 100%;
  height: 100%;
  position: relative;
  transition-property: transform;
}
.swiper-slide-invisible-blank {
  visibility: hidden;
}
/* Auto Height */
.swiper-container-autoheight,
.swiper-container-autoheight .swiper-slide {
  height: auto;
}
.swiper-container-autoheight .swiper-wrapper {
  align-items: flex-start;
  transition-property: transform, height;
}
/* 3D Effects */
.swiper-container-3d {
  perspective: 1200px;
}
.swiper-container-3d .swiper-wrapper,
.swiper-container-3d .swiper-slide,
.swiper-container-3d .swiper-slide-shadow-left,
.swiper-container-3d .swiper-slide-shadow-right,
.swiper-container-3d .swiper-slide-shadow-top,
.swiper-container-3d .swiper-slide-shadow-bottom,
.swiper-container-3d .swiper-cube-shadow {
  transform-style: preserve-3d;
}
.swiper-container-3d .swiper-slide-shadow-left,
.swiper-container-3d .swiper-slide-shadow-right,
.swiper-container-3d .swiper-slide-shadow-top,
.swiper-container-3d .swiper-slide-shadow-bottom {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 10;
}
.swiper-container-3d .swiper-slide-shadow-left {
  background-image: linear-gradient(to left, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}
.swiper-container-3d .swiper-slide-shadow-right {
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}
.swiper-container-3d .swiper-slide-shadow-top {
  background-image: linear-gradient(to top, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}
.swiper-container-3d .swiper-slide-shadow-bottom {
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}
/* CSS Mode */
.swiper-container-css-mode > .swiper-wrapper {
  overflow: auto;
  scrollbar-width: none;
  /* For Firefox */
  -ms-overflow-style: none;
  /* For Internet Explorer and Edge */
}
.swiper-container-css-mode > .swiper-wrapper::-webkit-scrollbar {
  display: none;
}
.swiper-container-css-mode > .swiper-wrapper > .swiper-slide {
  scroll-snap-align: start start;
}
.swiper-container-horizontal.swiper-container-css-mode > .swiper-wrapper {
  scroll-snap-type: x mandatory;
}
.swiper-container-vertical.swiper-container-css-mode > .swiper-wrapper {
  scroll-snap-type: y mandatory;
}
/* a11y */
.swiper-container .swiper-notification {
  position: absolute;
  left: 0;
  top: 0;
  pointer-events: none;
  opacity: 0;
  z-index: -1000;
}
.swiper-container-cube {
  overflow: visible;
}
.swiper-container-cube .swiper-slide {
  pointer-events: none;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  z-index: 1;
  visibility: hidden;
  transform-origin: 0 0;
  width: 100%;
  height: 100%;
}
.swiper-container-cube .swiper-slide .swiper-slide {
  pointer-events: none;
}
.swiper-container-cube.swiper-container-rtl .swiper-slide {
  transform-origin: 100% 0;
}
.swiper-container-cube .swiper-slide-active,
.swiper-container-cube .swiper-slide-active .swiper-slide-active {
  pointer-events: auto;
}
.swiper-container-cube .swiper-slide-active,
.swiper-container-cube .swiper-slide-next,
.swiper-container-cube .swiper-slide-prev,
.swiper-container-cube .swiper-slide-next + .swiper-slide {
  pointer-events: auto;
  visibility: visible;
}
.swiper-container-cube .swiper-slide-shadow-top,
.swiper-container-cube .swiper-slide-shadow-bottom,
.swiper-container-cube .swiper-slide-shadow-left,
.swiper-container-cube .swiper-slide-shadow-right {
  z-index: 0;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
.swiper-container-cube .swiper-cube-shadow {
  position: absolute;
  left: 0;
  bottom: 0px;
  width: 100%;
  height: 100%;
  background: #000;
  opacity: 0.6;
  -webkit-filter: blur(50px);
  filter: blur(50px);
  z-index: 0;
}
.swiper-container-fade.swiper-container-free-mode .swiper-slide {
  transition-timing-function: ease-out;
}
.swiper-container-fade .swiper-slide {
  pointer-events: none;
  transition-property: opacity;
}
.swiper-container-fade .swiper-slide .swiper-slide {
  pointer-events: none;
}
.swiper-container-fade .swiper-slide-active,
.swiper-container-fade .swiper-slide-active .swiper-slide-active {
  pointer-events: auto;
}
.swiper-container-flip {
  overflow: visible;
}
.swiper-container-flip .swiper-slide {
  pointer-events: none;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  z-index: 1;
}
.swiper-container-flip .swiper-slide .swiper-slide {
  pointer-events: none;
}
.swiper-container-flip .swiper-slide-active,
.swiper-container-flip .swiper-slide-active .swiper-slide-active {
  pointer-events: auto;
}
.swiper-container-flip .swiper-slide-shadow-top,
.swiper-container-flip .swiper-slide-shadow-bottom,
.swiper-container-flip .swiper-slide-shadow-left,
.swiper-container-flip .swiper-slide-shadow-right {
  z-index: 0;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
}
/* Preloader */
:root {
  /*
  --swiper-preloader-color: var(--swiper-theme-color);
  */
}
.swiper-lazy-preloader {
  width: 42px;
  height: 42px;
  position: absolute;
  left: 50%;
  top: 50%;
  margin-left: -21px;
  margin-top: -21px;
  z-index: 10;
  transform-origin: 50%;
  animation: swiper-preloader-spin 1s infinite linear;
  box-sizing: border-box;
  border: 4px solid var(--swiper-preloader-color, var(--swiper-theme-color));
  border-radius: 50%;
  border-top-color: transparent;
}
.swiper-lazy-preloader-white {
  --swiper-preloader-color: #fff;
}
.swiper-lazy-preloader-black {
  --swiper-preloader-color: #000;
}
@keyframes swiper-preloader-spin {
  100% {
    transform: rotate(360deg);
  }
}
:root {
  --swiper-navigation-size: 44px;
  /*
  --swiper-navigation-color: var(--swiper-theme-color);
  */
}
.swiper-button-prev,
.swiper-button-next {
  position: absolute;
  top: 50%;
  width: calc(var(--swiper-navigation-size) / 44 * 27);
  height: var(--swiper-navigation-size);
  margin-top: calc(-1 * var(--swiper-navigation-size) / 2);
  z-index: 10;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--swiper-navigation-color, var(--swiper-theme-color));
}
.swiper-button-prev.swiper-button-disabled,
.swiper-button-next.swiper-button-disabled {
  opacity: 0.35;
  cursor: auto;
  pointer-events: none;
}
.swiper-button-prev:after,
.swiper-button-next:after {
  font-family: swiper-icons;
  font-size: var(--swiper-navigation-size);
  text-transform: none !important;
}
.swiper-button-prev,
.swiper-container-rtl .swiper-button-next {
  left: 10px;
  right: auto;
}
.swiper-button-prev:after,
.swiper-container-rtl .swiper-button-next:after {
  content: 'prev';
}
.swiper-button-next,
.swiper-container-rtl .swiper-button-prev {
  right: 10px;
  left: auto;
}
.swiper-button-next:after,
.swiper-container-rtl .swiper-button-prev:after {
  content: 'next';
}
.swiper-button-lock {
  display: none;
}
:root {
  /*
  --swiper-pagination-color: var(--swiper-theme-color);
  */
}
.swiper-pagination {
  position: absolute;
  text-align: center;
  transition: 300ms opacity;
  transform: translate3d(0, 0, 0);
  z-index: 10;
}
.swiper-pagination.swiper-pagination-hidden {
  opacity: 0;
}
/* Common Styles */
.swiper-pagination-fraction,
.swiper-pagination-custom,
.swiper-container-horizontal > .swiper-pagination-bullets {
  bottom: 10px;
  left: 0;
  width: 100%;
}
/* Bullets */
.swiper-pagination-bullets-dynamic {
  overflow: hidden;
  font-size: 0;
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  transform: scale(0.33);
  position: relative;
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active {
  transform: scale(1);
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-main {
  transform: scale(1);
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-prev {
  transform: scale(0.66);
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-prev-prev {
  transform: scale(0.33);
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-next {
  transform: scale(0.66);
}
.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-next-next {
  transform: scale(0.33);
}
.swiper-pagination-bullet {
  width: 8px;
  height: 8px;
  display: inline-block;
  border-radius: 100%;
  background: #000;
  opacity: 0.2;
}
button.swiper-pagination-bullet {
  border: none;
  margin: 0;
  padding: 0;
  box-shadow: none;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
}
.swiper-pagination-clickable .swiper-pagination-bullet {
  cursor: pointer;
}
.swiper-pagination-bullet-active {
  opacity: 1;
  background: var(--swiper-pagination-color, var(--swiper-theme-color));
}
.swiper-container-vertical > .swiper-pagination-bullets {
  right: 10px;
  top: 50%;
  transform: translate3d(0px, -50%, 0);
}
.swiper-container-vertical > .swiper-pagination-bullets .swiper-pagination-bullet {
  margin: 6px 0;
  display: block;
}
.swiper-container-vertical > .swiper-pagination-bullets.swiper-pagination-bullets-dynamic {
  top: 50%;
  transform: translateY(-50%);
  width: 8px;
}
.swiper-container-vertical > .swiper-pagination-bullets.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  display: inline-block;
  transition: 200ms transform, 200ms top;
}
.swiper-container-horizontal > .swiper-pagination-bullets .swiper-pagination-bullet {
  margin: 0 4px;
}
.swiper-container-horizontal > .swiper-pagination-bullets.swiper-pagination-bullets-dynamic {
  left: 50%;
  transform: translateX(-50%);
  white-space: nowrap;
}
.swiper-container-horizontal > .swiper-pagination-bullets.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  transition: 200ms transform, 200ms left;
}
.swiper-container-horizontal.swiper-container-rtl > .swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  transition: 200ms transform, 200ms right;
}
/* Progress */
.swiper-pagination-progressbar {
  background: rgba(0, 0, 0, 0.25);
  position: absolute;
}
.swiper-pagination-progressbar .swiper-pagination-progressbar-fill {
  background: var(--swiper-pagination-color, var(--swiper-theme-color));
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  transform: scale(0);
  transform-origin: left top;
}
.swiper-container-rtl .swiper-pagination-progressbar .swiper-pagination-progressbar-fill {
  transform-origin: right top;
}
.swiper-container-horizontal > .swiper-pagination-progressbar,
.swiper-container-vertical > .swiper-pagination-progressbar.swiper-pagination-progressbar-opposite {
  width: 100%;
  height: 4px;
  left: 0;
  top: 0;
}
.swiper-container-vertical > .swiper-pagination-progressbar,
.swiper-container-horizontal > .swiper-pagination-progressbar.swiper-pagination-progressbar-opposite {
  width: 4px;
  height: 100%;
  left: 0;
  top: 0;
}
.swiper-pagination-lock {
  display: none;
}
/* Scrollbar */
.swiper-scrollbar {
  border-radius: 10px;
  position: relative;
  -ms-touch-action: none;
  background: rgba(0, 0, 0, 0.1);
}
.swiper-container-horizontal > .swiper-scrollbar {
  position: absolute;
  left: 1%;
  bottom: 3px;
  z-index: 50;
  height: 5px;
  width: 98%;
}
.swiper-container-vertical > .swiper-scrollbar {
  position: absolute;
  right: 3px;
  top: 1%;
  z-index: 50;
  width: 5px;
  height: 98%;
}
.swiper-scrollbar-drag {
  height: 100%;
  width: 100%;
  position: relative;
  background: rgba(0, 0, 0, 0.5);
  border-radius: 10px;
  left: 0;
  top: 0;
}
.swiper-scrollbar-cursor-drag {
  cursor: move;
}
.swiper-scrollbar-lock {
  display: none;
}
.swiper-zoom-container {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.swiper-zoom-container > img,
.swiper-zoom-container > svg,
.swiper-zoom-container > canvas {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}
.swiper-slide-zoomed {
  cursor: move;
}
:root {
  --swiper-theme-color: var(--f7-theme-color);
}
/* === Photo Browser === */
:root {
  --f7-photobrowser-bg-color: #fff;
  --f7-photobrowser-bars-bg-image: none;
  /*
  --f7-photobrowser-bars-bg-color: rgba(var(--f7-bars-bg-color-rgb), 0.95);
  --f7-photobrowser-bars-text-color: var(--f7-bars-text-color);
  --f7-photobrowser-bars-link-color: var(--f7-bars-link-color);
  */
  --f7-photobrowser-caption-font-size: 14px;
  --f7-photobrowser-caption-light-text-color: #000;
  --f7-photobrowser-caption-light-bg-color: rgba(255, 255, 255, 0.8);
  --f7-photobrowser-caption-dark-text-color: #fff;
  --f7-photobrowser-caption-dark-bg-color: rgba(0, 0, 0, 0.8);
  --f7-photobrowser-exposed-bg-color: #000;
  --f7-photobrowser-dark-bg-color: #000;
  --f7-photobrowser-dark-bars-bg-color: rgba(27, 27, 27, 0.8);
  --f7-photobrowser-dark-bars-text-color: #fff;
  --f7-photobrowser-dark-bars-link-color: #fff;
}
.photo-browser {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  z-index: 400;
}
.photo-browser-standalone.modal-in {
  transition-duration: 0ms;
  animation: photo-browser-in 400ms;
}
.photo-browser-standalone.modal-out {
  transition-duration: 0ms;
  animation: photo-browser-out 400ms !important;
}
.photo-browser-standalone.modal-out.swipe-close-to-bottom,
.photo-browser-standalone.modal-out.swipe-close-to-top {
  animation: none !important;
}
.photo-browser-standalone.photo-browser-transitioning {
  transition: 400ms;
  transition-property: transform;
  animation: none !important;
}
.photo-browser-popup.modal-out.swipe-close-to-bottom,
.photo-browser-popup.modal-out.swipe-close-to-top {
  transition-duration: 300ms;
}
.photo-browser-popup.modal-out.swipe-close-to-bottom {
  transform: translate3d(0, 100%, 0);
}
.photo-browser-popup.modal-out.swipe-close-to-top {
  transform: translate3d(0, -100vh, 0);
}
.photo-browser-page {
  background: none;
}
.photo-browser-page .toolbar {
  transform: none;
}
.photo-browser-popup {
  background: none;
}
.photo-browser-of {
  margin: 0 5px;
}
.photo-browser-captions {
  pointer-events: none;
  position: absolute;
  left: 0;
  width: 100%;
  bottom: var(--f7-safe-area-bottom);
  z-index: 10;
  opacity: 1;
  transition: 400ms;
}
.photo-browser-captions.photo-browser-captions-exposed {
  opacity: 0;
}
.toolbar ~ .photo-browser-captions {
  bottom: calc(var(--f7-toolbar-height) + var(--f7-safe-area-bottom));
  transform: translate3d(0, 0px, 0);
}
.toolbar ~ .photo-browser-captions.photo-browser-captions-exposed {
  transform: translate3d(0, 0px, 0);
}
.photo-browser-caption {
  box-sizing: border-box;
  transition: 300ms;
  position: absolute;
  bottom: 0;
  left: 0;
  opacity: 0;
  padding: 4px 5px;
  width: 100%;
  text-align: center;
  font-size: var(--f7-photobrowser-caption-font-size);
}
.photo-browser-caption:empty {
  display: none;
}
.photo-browser-caption.photo-browser-caption-active {
  opacity: 1;
}
.photo-browser-captions-light .photo-browser-caption {
  color: var(--f7-photobrowser-caption-light-text-color);
  background: var(--f7-photobrowser-caption-light-bg-color);
}
.photo-browser-captions-dark .photo-browser-caption {
  color: var(--f7-photobrowser-caption-dark-text-color);
  background: var(--f7-photobrowser-caption-dark-bg-color);
}
.photo-browser-swiper-container {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  background: var(--f7-photobrowser-bg-color);
  transition: 400ms;
  transition-property: background-color;
}
.photo-browser-prev.swiper-button-disabled,
.photo-browser-next.swiper-button-disabled {
  opacity: 0.3;
  pointer-events: none;
}
.photo-browser-slide {
  width: 100%;
  height: 100%;
  position: relative;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  box-sizing: border-box;
}
.photo-browser-slide span.swiper-zoom-container {
  display: none;
}
.photo-browser-slide img {
  width: auto;
  height: auto;
  max-width: 100%;
  max-height: 100%;
  display: none;
}
.photo-browser-slide.swiper-slide-active span.swiper-zoom-container,
.photo-browser-slide.swiper-slide-next span.swiper-zoom-container,
.photo-browser-slide.swiper-slide-prev span.swiper-zoom-container {
  display: flex;
}
.photo-browser-slide.swiper-slide-active img,
.photo-browser-slide.swiper-slide-next img,
.photo-browser-slide.swiper-slide-prev img {
  display: inline;
}
.photo-browser-slide.swiper-slide-active.photo-browser-slide-lazy .preloader,
.photo-browser-slide.swiper-slide-next.photo-browser-slide-lazy .preloader,
.photo-browser-slide.swiper-slide-prev.photo-browser-slide-lazy .preloader {
  display: block;
}
.photo-browser-slide iframe {
  width: 100%;
  height: 100%;
}
.photo-browser-slide .preloader {
  display: none;
  position: absolute;
  width: 42px;
  height: 42px;
  margin-left: -21px;
  margin-top: -21px;
  left: 50%;
  top: 50%;
}
.photo-browser-page .navbar-bg,
.navbar-photo-browser .navbar-bg,
.photo-browser-page .toolbar {
  background-color: var(--f7-photobrowser-bars-bg-color, rgba(var(--f7-bars-bg-color-rgb), 0.95));
  background-image: var(--f7-photobrowser-bars-bg-image);
}
.photo-browser-page .navbar,
.photo-browser-page .toolbar {
  transition: 400ms;
  color: var(--f7-photobrowser-bars-text-color, var(--f7-bars-text-color));
}
.photo-browser-page .navbar a,
.photo-browser-page .toolbar a {
  color: var(--f7-photobrowser-bars-link-color, var(--f7-bars-link-color, var(--f7-theme-color)));
}
.photo-browser-exposed .navbar,
.photo-browser-exposed .toolbar {
  opacity: 0;
  visibility: hidden;
  pointer-events: none;
}
.photo-browser-exposed .toolbar ~ .photo-browser-captions {
  transform: translate3d(0, var(--f7-toolbar-height), 0);
}
.photo-browser-exposed .photo-browser-swiper-container {
  background: var(--f7-photobrowser-exposed-bg-color);
}
.photo-browser-exposed .photo-browser-caption {
  color: var(--f7-photobrowser-caption-dark-text-color);
  background: var(--f7-photobrowser-caption-dark-bg-color);
}
.view.with-photo-browser-page-exposed .navbar {
  opacity: 0;
  pointer-events: none;
}
.photo-browser-page-dark .navbar-bg,
.navbar-photo-browser-dark .navbar-bg,
.photo-browser-page-dark .toolbar {
  background: var(--f7-photobrowser-dark-bars-bg-color);
}
.photo-browser-page-dark .navbar-bg:before,
.navbar-photo-browser-dark .navbar-bg:before,
.photo-browser-page-dark .toolbar:before,
.photo-browser-page-dark .navbar-bg:after,
.navbar-photo-browser-dark .navbar-bg:after,
.photo-browser-page-dark .toolbar:after {
  display: none !important;
}
.navbar-photo-browser-dark,
.photo-browser-dark .navbar,
.photo-browser-dark .toolbar,
.photo-browser-dark-page .navbar,
.photo-browser-dark-page .toolbar {
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
  --f7-link-highlight-color: var(--f7-link-highlight-white);
  color: var(--f7-photobrowser-dark-bars-text-color);
}
.navbar-photo-browser-dark a,
.photo-browser-dark .navbar a,
.photo-browser-dark .toolbar a,
.photo-browser-dark-page .navbar a,
.photo-browser-dark-page .toolbar a {
  color: var(--f7-photobrowser-dark-bars-link-color);
}
.photo-browser-dark .photo-browser-swiper-container,
.photo-browser-page-dark .photo-browser-swiper-container {
  background: var(--f7-photobrowser-dark-bg-color);
}
@keyframes photo-browser-in {
  0% {
    transform: translate3d(0, 0, 0) scale(0.5);
    opacity: 0;
  }
  50% {
    transform: translate3d(0, 0, 0) scale(1.05);
    opacity: 1;
  }
  100% {
    transform: translate3d(0, 0, 0) scale(1);
    opacity: 1;
  }
}
@keyframes photo-browser-out {
  0% {
    transform: translate3d(0, 0, 0) scale(1);
    opacity: 1;
  }
  50% {
    transform: translate3d(0, 0, 0) scale(1.05);
    opacity: 1;
  }
  100% {
    transform: translate3d(0, 0, 0) scale(0.5);
    opacity: 0;
  }
}
/* === Notifications === */
:root {
  --f7-notification-max-width: 568px;
  --f7-notification-subtitle-text-transform: none;
  --f7-notification-subtitle-line-height: 1.35;
  --f7-notification-text-text-transform: none;
  --f7-notification-text-font-weight: 400;
}
:root .theme-dark,
:root.theme-dark {
  --f7-notification-subtitle-color: #fff;
}
.ios {
  --f7-notification-margin: 8px;
  --f7-notification-padding: 10px;
  --f7-notification-border-radius: 12px;
  --f7-notification-box-shadow: 0px 5px 25px -10px rgba(0, 0, 0, 0.7);
  --f7-notification-icon-size: 20px;
  --f7-notification-title-font-size: 13px;
  --f7-notification-title-text-transform: uppercase;
  --f7-notification-title-line-height: 1.4;
  --f7-notification-title-font-weight: 400;
  --f7-notification-title-letter-spacing: 0.02em;
  --f7-notification-title-right-font-size: 13px;
  --f7-notification-subtitle-font-size: 15px;
  --f7-notification-subtitle-font-weight: 600;
  --f7-notification-text-font-size: 15px;
  --f7-notification-text-line-height: 1.2;
  --f7-notification-bg-color: rgba(250, 250, 250, 0.95);
  --f7-notification-bg-color-rgb: 255, 255, 255;
  --f7-notification-title-color: #000;
  --f7-notification-title-right-color: rgba(0, 0, 0, 0.45);
  --f7-notification-subtitle-color: #000;
  --f7-notification-text-color: #000;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-notification-bg-color: rgba(30, 30, 30, 0.95);
  --f7-notification-bg-color-rgb: 30, 30, 30;
  --f7-notification-title-color: #fff;
  --f7-notification-text-color: #fff;
  --f7-notification-title-right-color: rgba(255, 255, 255, 0.55);
}
.md {
  --f7-notification-margin: 0px;
  --f7-notification-padding: 16px;
  --f7-notification-border-radius: 0px;
  --f7-notification-box-shadow: 0 2px 4px rgba(0, 0, 0, 0.22), 0 1px 2px rgba(0, 0, 0, 0.24);
  --f7-notification-icon-size: 16px;
  --f7-notification-title-color: var(--f7-theme-color);
  --f7-notification-title-font-size: 12px;
  --f7-notification-title-text-transform: none;
  --f7-notification-title-line-height: 1;
  --f7-notification-title-font-weight: 400;
  --f7-notification-title-right-font-size: 12px;
  --f7-notification-subtitle-font-size: 14px;
  --f7-notification-subtitle-font-weight: 400;
  --f7-notification-text-font-size: 14px;
  --f7-notification-text-line-height: 1.35;
  --f7-notification-bg-color: #fff;
  --f7-notification-title-right-color: rgba(0, 0, 0, 0.54);
  --f7-notification-subtitle-color: #212121;
  --f7-notification-text-color: rgba(0, 0, 0, 0.54);
}
.md .theme-dark,
.md.theme-dark {
  --f7-notification-bg-color: #242424;
  --f7-notification-title-right-color: rgba(255, 255, 255, 0.54);
  --f7-notification-text-color: rgba(255, 255, 255, 0.54);
}
.aurora {
  --f7-notification-margin: 10px;
  --f7-notification-padding: 10px;
  --f7-notification-border-radius: 4px;
  --f7-notification-box-shadow: 0px 5px 25px -10px rgba(0, 0, 0, 0.7);
  --f7-notification-icon-size: 18px;
  --f7-notification-title-font-size: 13px;
  --f7-notification-title-text-transform: uppercase;
  --f7-notification-title-line-height: 1.4;
  --f7-notification-title-font-weight: 500;
  --f7-notification-title-letter-spacing: 0.02em;
  --f7-notification-title-right-font-size: 13px;
  --f7-notification-subtitle-font-size: 12px;
  --f7-notification-subtitle-font-weight: 600;
  --f7-notification-text-font-size: 12px;
  --f7-notification-text-line-height: 1.2;
  --f7-notification-bg-color: #fff;
  --f7-notification-title-color: #000;
  --f7-notification-title-right-color: rgba(255, 255, 255, 0.6);
  --f7-notification-subtitle-color: #000;
  --f7-notification-text-color: #000;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-notification-bg-color: #242424;
  --f7-notification-title-color: #fff;
  --f7-notification-text-color: #fff;
  --f7-notification-title-right-color: rgba(255, 255, 255, 0.54);
}
.notification {
  --f7-link-highlight-color: var(--f7-link-highlight-black);
  --f7-touch-ripple-color: var(--f7-touch-ripple-black);
  position: absolute;
  left: var(--f7-notification-margin);
  top: var(--f7-notification-margin);
  width: calc(100% - var(--f7-notification-margin) * 2);
  z-index: 20000;
  font-size: 14px;
  margin: 0;
  border: none;
  display: none;
  box-sizing: border-box;
  transition-property: transform;
  direction: ltr;
  max-width: var(--f7-notification-max-width);
  padding: var(--f7-notification-padding);
  border-radius: var(--f7-notification-border-radius);
  box-shadow: var(--f7-notification-box-shadow);
  background: var(--f7-notification-bg-color);
  margin-top: var(--f7-safe-area-top);
}
@supports ((-webkit-backdrop-filter: blur(20px)) or (backdrop-filter: blur(20px))) {
  .ios-translucent-modals .notification {
    background-color: rgba(var(--f7-notification-bg-color-rgb), 0.8);
    -webkit-backdrop-filter: saturate(180%) blur(20px);
            backdrop-filter: saturate(180%) blur(20px);
  }
}
@media (min-width: 568px) {
  .notification {
    left: 50%;
    width: var(--f7-notification-max-width);
    margin-left: calc(-1 * var(--f7-notification-max-width) / 2);
  }
}
.notification-title {
  color: var(--f7-notification-title-color, var(--f7-theme-color));
  font-size: var(--f7-notification-title-font-size);
  text-transform: var(--f7-notification-title-text-transform);
  line-height: var(--f7-notification-title-line-height);
  font-weight: var(--f7-notification-title-font-weight);
  letter-spacing: var(--f7-notification-title-letter-spacing);
}
.notification-subtitle {
  color: var(--f7-notification-subtitle-color);
  font-size: var(--f7-notification-subtitle-font-size);
  text-transform: var(--f7-notification-subtitle-text-transform);
  line-height: var(--f7-notification-subtitle-line-height);
  font-weight: var(--f7-notification-subtitle-font-weight);
}
.notification-text {
  color: var(--f7-notification-text-color);
  font-size: var(--f7-notification-text-font-size);
  text-transform: var(--f7-notification-text-text-transform);
  line-height: var(--f7-notification-text-line-height);
  font-weight: var(--f7-notification-text-font-weight);
}
.notification-title-right-text {
  color: var(--f7-notification-title-right-color);
  font-size: var(--f7-notification-title-right-font-size);
}
.notification-icon {
  font-size: 0;
  line-height: var(--f7-notification-icon-size);
}
.notification-icon i,
.notification-icon {
  width: var(--f7-notification-icon-size) !important;
  height: var(--f7-notification-icon-size) !important;
}
.notification-icon i {
  font-size: var(--f7-notification-icon-size);
}
.notification-header {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
.notification-close-button {
  margin-left: auto;
  cursor: pointer;
  position: relative;
}
.notification-close-button:after {
  font-family: 'framework7-core-icons';
  font-weight: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale;
  -moz-font-feature-settings: "liga";
       font-feature-settings: "liga";
  display: block;
  width: 100%;
  height: 100%;
  font-size: 20px;
  position: absolute;
  left: 50%;
  top: 50%;
  text-align: center;
}
.ios .notification {
  transition-duration: 450ms;
  transform: translate3d(0%, -200%, 0);
}
.ios .notification.modal-in {
  transform: translate3d(0%, 0%, 0);
  opacity: 1;
}
.ios .notification.modal-out {
  transform: translate3d(0%, -200%, 0);
}
.ios .notification-icon {
  margin-right: 8px;
}
.ios .notification-header + .notification-content {
  margin-top: 10px;
}
.ios .notification-title-right-text {
  margin-right: 6px;
  margin-left: auto;
}
.ios .notification-title-right-text + .notification-close-button {
  margin-left: 10px;
}
.ios .notification-close-button {
  font-size: 14px;
  width: 20px;
  height: 20px;
  opacity: 0.3;
  transition-duration: 300ms;
}
.ios .notification-close-button.active-state {
  transition-duration: 0ms;
  opacity: 0.1;
}
.ios .notification-close-button:after {
  color: #000;
  content: 'notification_close_ios';
  font-size: 0.65em;
  line-height: 44px;
  width: 44px;
  height: 44px;
  margin-left: -22px;
  margin-top: -22px;
}
.ios .theme-dark .notification-close-button:after,
.ios.theme-dark .notification-close-button:after {
  color: #fff;
}
.md .notification {
  transform: translate3d(0, -150%, 0);
}
.md .notification.modal-in {
  transition-duration: 0ms;
  animation: notification-md-in 400ms ease-out;
  transform: translate3d(0, 0%, 0);
}
.md .notification.modal-in.notification-transitioning {
  transition-duration: 200ms;
}
.md .notification.modal-out {
  animation: none;
  transition-duration: 200ms;
  transition-timing-function: ease-in;
  transform: translate3d(0, -150%, 0);
}
.md .notification-icon {
  margin-right: 8px;
}
.md .notification-subtitle + .notification-text {
  margin-top: 2px;
}
.md .notification-header + .notification-content {
  margin-top: 6px;
}
.md .notification-title-right-text {
  margin-left: 4px;
}
.md .notification-title-right-text:before {
  content: '';
  width: 3px;
  height: 3px;
  border-radius: 50%;
  display: inline-block;
  vertical-align: middle;
  margin-right: 4px;
  background: var(--f7-notification-title-right-color);
}
.md .notification-close-button {
  width: 16px;
  height: 16px;
  transition-duration: 300ms;
}
.md .notification-close-button:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md .notification-close-button.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .notification-close-button:before,
.md .notification-close-button:after {
  width: 48px;
  height: 48px;
  left: 50%;
  top: 50%;
  margin-left: -24px;
  margin-top: -24px;
}
.md .notification-close-button:after {
  color: #737373;
  content: 'delete_md';
  line-height: 48px;
  font-size: 14px;
}
@keyframes notification-md-in {
  0% {
    transform: translate3d(0, -150%, 0);
  }
  50% {
    transform: translate3d(0, 10%, 0);
  }
  100% {
    transform: translate3d(0, 0%, 0);
  }
}
.aurora .notification {
  transition-duration: 450ms;
  transform: translate3d(0%, -200%, 0);
}
.aurora .notification.modal-in {
  transform: translate3d(0%, 0%, 0);
  opacity: 1;
}
.aurora .notification.modal-out {
  transform: translate3d(0%, -200%, 0);
}
.aurora .notification-icon {
  margin-right: 10px;
}
.aurora .notification-header + .notification-content {
  margin-top: 10px;
}
.aurora .notification-title-right-text {
  margin-right: 0px;
  margin-left: auto;
}
.aurora .notification-title-right-text + .notification-close-button {
  margin-left: 10px;
}
.aurora .notification-close-button {
  font-size: 14px;
  width: 16px;
  height: 16px;
  opacity: 0.4;
  transition-duration: 300ms;
}
.aurora .notification-close-button.active-state {
  transition-duration: 0ms;
  opacity: 0.6;
}
.aurora .notification-close-button:after {
  color: #000;
  content: 'notification_close_ios';
  font-size: 0.5em;
  line-height: 38px;
  width: 38px;
  height: 38px;
  margin-left: -19px;
  margin-top: -19px;
}
.aurora .theme-dark .notification-close-button:after,
.aurora.theme-dark .notification-close-button:after {
  color: #fff;
}
/* === Autocomplete === */
:root {
  --f7-autocomplete-dropdown-placeholder-color: #a9a9a9;
  --f7-autocomplete-dropdown-preloader-size: 20px;
  /*
  --f7-autocomplete-dropdown-selected-bg-color: rgba(var(--f7-theme-color-rgb), 0.2);
  */
  --f7-autocomplete-dropdown-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-autocomplete-dropdown-bg-color: #1c1c1d;
}
.ios {
  --f7-autocomplete-dropdown-box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.2);
  --f7-autocomplete-dropdown-text-matching-font-weight: 600;
  --f7-autocomplete-dropdown-font-size: var(--f7-list-font-size);
  --f7-autocomplete-dropdown-text-color: #000;
  --f7-autocomplete-dropdown-text-matching-color: #000;
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-autocomplete-dropdown-text-color: #fff;
  --f7-autocomplete-dropdown-text-matching-color: #fff;
}
.md {
  --f7-autocomplete-dropdown-box-shadow: 0 2px 2px rgba(0, 0, 0, 0.25);
  --f7-autocomplete-dropdown-text-matching-font-weight: 400;
  --f7-autocomplete-dropdown-font-size: var(--f7-list-font-size);
  --f7-autocomplete-dropdown-text-color: rgba(0, 0, 0, 0.54);
  --f7-autocomplete-dropdown-text-matching-color: #212121;
}
.md .theme-dark,
.md.theme-dark {
  --f7-autocomplete-dropdown-text-color: rgba(255, 255, 255, 0.54);
  --f7-autocomplete-dropdown-text-matching-color: rgba(255, 255, 255, 0.87);
}
.aurora {
  --f7-autocomplete-dropdown-box-shadow: 0px 1px 2px rgba(0, 0, 0, 0.2);
  --f7-autocomplete-dropdown-text-matching-font-weight: 700;
  --f7-autocomplete-dropdown-font-size: 13px;
  --f7-autocomplete-dropdown-text-color: #000;
  --f7-autocomplete-dropdown-text-matching-color: #000;
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-autocomplete-dropdown-text-color: #fff;
  --f7-autocomplete-dropdown-text-matching-color: #fff;
}
.autocomplete-page .autocomplete-found {
  display: block;
}
.autocomplete-page .autocomplete-not-found {
  display: none;
}
.autocomplete-page .autocomplete-values {
  display: block;
}
.autocomplete-page .list ul:empty {
  display: none;
}
.autocomplete-preloader:not(.autocomplete-preloader-visible) {
  visibility: hidden;
}
.autocomplete-preloader:not(.autocomplete-preloader-visible),
.autocomplete-preloader:not(.autocomplete-preloader-visible) * {
  animation: none;
}
.autocomplete-dropdown {
  background: var(--f7-autocomplete-dropdown-bg-color);
  box-shadow: var(--f7-autocomplete-dropdown-box-shadow);
  box-sizing: border-box;
  position: absolute;
  z-index: 500;
  width: 100%;
  left: 0;
}
.autocomplete-dropdown .autocomplete-dropdown-inner {
  position: relative;
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  height: 100%;
  z-index: 1;
}
.autocomplete-dropdown .autocomplete-preloader {
  display: none;
  position: absolute;
  bottom: 100%;
  width: var(--f7-autocomplete-dropdown-preloader-size);
  height: var(--f7-autocomplete-dropdown-preloader-size);
}
.autocomplete-dropdown .autocomplete-preloader-visible {
  display: block;
}
.autocomplete-dropdown .autocomplete-dropdown-placeholder {
  color: var(--f7-autocomplete-dropdown-placeholder-color);
}
.autocomplete-dropdown .list {
  margin: 0;
  color: var(--f7-autocomplete-dropdown-text-color);
  font-size: var(--f7-autocomplete-dropdown-font-size);
}
.autocomplete-dropdown .list b {
  color: var(--f7-autocomplete-dropdown-text-matching-color);
  font-weight: var(--f7-autocomplete-dropdown-text-matching-font-weight);
}
.autocomplete-dropdown .list ul {
  background: none !important;
}
.autocomplete-dropdown .list ul:before,
.autocomplete-dropdown .list ul:after {
  display: none !important;
}
.autocomplete-dropdown .autocomplete-dropdown-selected {
  background: var(--f7-autocomplete-dropdown-selected-bg-color, rgba(var(--f7-theme-color-rgb), 0.2));
}
.searchbar-input-wrap .autocomplete-dropdown {
  background-color: var(--f7-searchbar-input-bg-color, var(--f7-searchbar-bg-color));
  border-radius: var(--f7-searchbar-input-border-radius);
}
.searchbar-input-wrap .autocomplete-dropdown .autocomplete-dropdown-placeholder {
  color: var(--f7-searchbar-placeholder-color);
}
.searchbar-input-wrap .autocomplete-dropdown li:last-child {
  border-radius: 0 0 var(--f7-searchbar-input-border-radius) var(--f7-searchbar-input-border-radius);
  position: relative;
  overflow: hidden;
}
.searchbar-input-wrap .autocomplete-dropdown .item-content {
  padding-left: var(--f7-searchbar-input-padding-horizontal);
}
.list .item-content-dropdown-expanded .item-title.item-label {
  width: 0;
  flex-shrink: 10;
  overflow: hidden;
}
.list .item-content-dropdown-expanded .item-title.item-label + .item-input-wrap {
  margin-left: 0;
}
.list .item-content-dropdown-expanded .item-input-wrap {
  width: 100%;
}
.ios .autocomplete-dropdown .autocomplete-preloader {
  right: 16px;
  margin-bottom: 12px;
}
.ios .searchbar-input-wrap .autocomplete-dropdown {
  margin-top: calc(-1 * var(--f7-searchbar-input-height));
  top: 100%;
  z-index: 20;
}
.ios .searchbar-input-wrap .autocomplete-dropdown .autocomplete-dropdown-inner {
  padding-top: var(--f7-searchbar-input-height);
}
.md .autocomplete-page .navbar .autocomplete-preloader {
  margin-right: 8px;
}
.md .autocomplete-popup .navbar .autocomplete-preloader {
  margin-left: 8px;
  margin-right: 16px;
}
.md .autocomplete-dropdown .autocomplete-preloader {
  right: 16px;
  margin-bottom: 8px;
}
.md .autocomplete-dropdown .autocomplete-preloader .preloader-inner-gap,
.md .autocomplete-dropdown .autocomplete-preloader .preloader-inner-half-circle {
  border-width: 3px;
}
.aurora .autocomplete-dropdown .autocomplete-preloader {
  right: 16px;
  margin-bottom: 2px;
}
.aurora .searchbar-input-wrap .autocomplete-dropdown {
  margin-top: calc(-1 * var(--f7-searchbar-input-height));
  top: 100%;
  z-index: 20;
}
.aurora .searchbar-input-wrap .autocomplete-dropdown .autocomplete-dropdown-inner {
  padding-top: var(--f7-searchbar-input-height);
}
/* === Tooltip === */
:root {
  --f7-tooltip-bg-color: rgba(0, 0, 0, 0.87);
  --f7-tooltip-text-color: #fff;
  --f7-tooltip-border-radius: 4px;
  --f7-tooltip-padding: 8px 16px;
  --f7-tooltip-font-size: 14px;
  --f7-tooltip-font-weight: 500;
  --f7-tooltip-desktop-padding: 6px 8px;
  --f7-tooltip-desktop-font-size: 12px;
}
.tooltip {
  position: absolute;
  z-index: 20000;
  background: var(--f7-tooltip-bg-color);
  border-radius: var(--f7-tooltip-border-radius);
  padding: var(--f7-tooltip-padding);
  color: var(--f7-tooltip-text-color);
  font-size: var(--f7-tooltip-font-size);
  font-weight: var(--f7-tooltip-font-weight);
  box-sizing: border-box;
  line-height: 1.2;
  opacity: 0;
  transform: scale(0.9);
  transition-duration: 150ms;
  transition-property: opacity, transform;
  z-index: 99000;
}
.tooltip.tooltip-in {
  transform: scale(1);
  opacity: 1;
}
.tooltip.tooltip-out {
  opacity: 0;
  transform: scale(1);
}
.device-desktop .tooltip {
  font-size: var(--f7-tooltip-desktop-font-size);
  padding: var(--f7-tooltip-desktop-padding);
}
/* === Gauge === */
.gauge {
  position: relative;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
  display: inline-block;
}
.gauge-svg,
.gauge svg {
  max-width: 100%;
  height: auto;
}
.gauge-svg circle,
.gauge svg circle,
.gauge-svg path,
.gauge svg path {
  transition-duration: 400ms;
}
/* === Skeleton === */
:root {
  --f7-skeleton-color: #ccc;
}
.theme-dark {
  --f7-skeleton-color: #515151;
}
.skeleton-text {
  font-family: 'framework7-skeleton' !important;
}
.skeleton-text,
.skeleton-text * {
  color: var(--f7-skeleton-color) !important;
  font-weight: normal !important;
  font-style: normal !important;
  letter-spacing: -0.015em !important;
}
.skeleton-block {
  height: 1em;
  background: var(--f7-skeleton-color) !important;
  width: 100%;
}
.skeleton-effect-fade {
  animation: skeleton-effect-fade 1s infinite;
}
.skeleton-effect-blink {
  -webkit-mask-image: linear-gradient(to right, transparent 0%, black 25%, black 75%, transparent 100%);
  mask-image: linear-gradient(to right, transparent 0%, black 25%, black 75%, transparent 100%);
  -webkit-mask-size: 200% 100%;
  mask-size: 200% 100%;
  -webkit-mask-repeat: repeat;
  mask-repeat: repeat;
  -webkit-mask-position: 50% top;
  mask-position: 50% top;
  animation: skeleton-effect-blink 1s infinite;
}
.skeleton-effect-pulse {
  animation: skeleton-effect-pulse 1s infinite;
}
@keyframes skeleton-effect-fade {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0.2;
  }
  100% {
    opacity: 1;
  }
}
@keyframes skeleton-effect-blink {
  0% {
    -webkit-mask-position: 50% top;
    mask-position: 50% top;
  }
  100% {
    -webkit-mask-position: -150% top;
    mask-position: -150% top;
  }
}
@keyframes skeleton-effect-pulse {
  0% {
    transform: scale(1);
  }
  40% {
    transform: scale(1);
  }
  50% {
    transform: scale(0.975);
  }
  100% {
    transform: scale(1);
  }
}
/* === Menu === */
:root {
  --f7-menu-text-color: #fff;
  --f7-menu-font-size: 16px;
  --f7-menu-font-weight: 500;
  --f7-menu-line-height: 1.2;
  --f7-menu-bg-color: rgba(0, 0, 0, 0.9);
  --f7-menu-item-pressed-bg-color: rgba(20, 20, 20, 0.9);
  --f7-menu-item-padding-horizontal: 12px;
  --f7-menu-item-spacing: 6px;
  --f7-menu-item-height: 40px;
  --f7-menu-item-dropdown-icon-color: rgba(255, 255, 255, 0.4);
  --f7-menu-item-border-radius: 8px;
  /*
  --f7-menu-dropdown-pressed-bg-color: var(--f7-theme-color);
  */
  --f7-menu-dropdown-item-height: 28px;
  --f7-menu-dropdown-divider-color: rgba(255, 255, 255, 0.2);
  --f7-menu-dropdown-padding-vertical: 6px;
  /*
  --f7-menu-dropdown-border-radius: var(--f7-menu-item-border-radius);
  */
}
.aurora {
  --f7-menu-font-size: 13px;
  --f7-menu-item-height: 28px;
  --f7-menu-dropdown-item-height: 24px;
  --f7-menu-item-border-radius: 5px;
  --f7-menu-item-padding-horizontal: 10px;
}
.menu {
  z-index: 1000;
  position: relative;
  transform: translate3d(0, 0, 0);
  --f7-touch-ripple-color: var(--f7-touch-ripple-white);
}
.menu-inner {
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  padding-left: var(--f7-menu-item-spacing);
  padding-right: var(--f7-menu-item-spacing);
}
.menu-inner:after {
  content: '';
  width: var(--f7-menu-item-spacing);
  height: 100%;
  flex-shrink: 0;
}
.menu-item {
  height: var(--f7-menu-item-height);
  min-width: var(--f7-menu-item-height);
  flex-shrink: 0;
  background: var(--f7-menu-bg-color);
  color: var(--f7-menu-text-color);
  border-radius: var(--f7-menu-item-border-radius);
  position: relative;
  box-sizing: border-box;
  font-size: var(--f7-menu-font-size);
  font-weight: var(--f7-menu-font-weight);
  cursor: pointer;
  margin-left: var(--f7-menu-item-spacing);
}
.menu-item:first-child {
  margin-left: 0;
}
.menu-item.active-state:not(.menu-item-dropdown-opened) {
  background-color: rgba(0, 0, 0, 0.7);
}
.menu-item.icon-only {
  padding-left: 0;
  padding-right: 0;
}
.menu-item-content {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 var(--f7-menu-item-padding-horizontal);
  height: 100%;
  box-sizing: border-box;
  width: 100%;
  overflow: hidden;
  border-radius: var(--f7-menu-item-border-radius);
  position: relative;
}
.menu-item-content.icon-only,
.icon-only .menu-item-content {
  padding-left: 0;
  padding-right: 0;
}
.menu-item-dropdown .menu-item-content:after {
  content: '';
  position: absolute;
  width: 20px;
  height: 2px;
  left: 50%;
  transform: translateX(-50%);
  bottom: 4px;
  background: var(--f7-menu-item-dropdown-icon-color);
  border-radius: 4px;
}
.menu-dropdown {
  opacity: 0;
  visibility: hidden;
  pointer-events: none;
  cursor: auto;
  height: 10px;
  background: var(--f7-menu-bg-color);
  position: relative;
}
.menu-dropdown-content {
  position: absolute;
  top: 100%;
  border-radius: var(--f7-menu-dropdown-border-radius, var(--f7-menu-item-border-radius));
  padding-top: var(--f7-menu-dropdown-padding-vertical);
  padding-bottom: var(--f7-menu-dropdown-padding-vertical);
  box-sizing: border-box;
  background: var(--f7-menu-bg-color);
  overflow: auto;
  -webkit-overflow-scrolling: touch;
  min-width: calc(100% + 24px);
}
.menu-dropdown-link,
.menu-dropdown-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-left: var(--f7-menu-item-padding-horizontal);
  padding-right: var(--f7-menu-item-padding-horizontal);
  min-height: var(--f7-menu-dropdown-item-height);
  line-height: var(--f7-menu-line-height);
  font-size: var(--f7-menu-font-size);
  color: var(--f7-menu-text-color);
  font-weight: var(--f7-menu-font-weight);
  white-space: nowrap;
  min-width: 100px;
}
.menu-dropdown-link i,
.menu-dropdown-item i,
.menu-dropdown-link i.icon,
.menu-dropdown-item i.icon,
.menu-dropdown-link i.f7-icons,
.menu-dropdown-item i.f7-icons,
.menu-dropdown-link i.material-icons,
.menu-dropdown-item i.material-icons {
  font-size: 20px;
}
.menu-dropdown-link.active-state {
  background: var(--f7-menu-dropdown-pressed-bg-color, var(--f7-theme-color));
  color: var(--f7-menu-text-color);
}
.menu-dropdown-divider {
  height: 1px;
  margin-top: 2px;
  margin-bottom: 2px;
  background: var(--f7-menu-dropdown-divider-color);
}
.menu-item-dropdown-opened {
  border-bottom-left-radius: 0px;
  border-bottom-right-radius: 0px;
}
.menu-item-dropdown-opened .menu-item-content:after {
  opacity: 0;
}
.menu-item-dropdown-opened .menu-dropdown {
  opacity: 1;
  visibility: visible;
  pointer-events: auto;
}
.menu-item-dropdown-left .menu-dropdown:after,
.menu-item-dropdown-center .menu-dropdown:after,
.menu-dropdown-left:after,
.menu-dropdown-center:after {
  content: '';
  position: absolute;
  left: 100%;
  bottom: 0;
  width: var(--f7-menu-item-border-radius);
  height: var(--f7-menu-item-border-radius);
  background-image: radial-gradient(ellipse at 100% 0%, transparent 0%, transparent 70%, var(--f7-menu-bg-color) 72%);
}
.menu-item-dropdown-right .menu-dropdown:before,
.menu-item-dropdown-center .menu-dropdown:before,
.menu-dropdown-right:before,
.menu-dropdown-center:before {
  content: '';
  position: absolute;
  right: 100%;
  bottom: 0;
  width: var(--f7-menu-item-border-radius);
  height: var(--f7-menu-item-border-radius);
  background-image: radial-gradient(ellipse at 0% 0%, transparent 0%, transparent 70%, var(--f7-menu-bg-color) 72%);
}
.menu-item-dropdown-left .menu-dropdown-content,
.menu-dropdown-left .menu-dropdown-content {
  left: 0;
  border-top-left-radius: 0px;
}
.menu-item-dropdown-right .menu-dropdown-content,
.menu-dropdown-right .menu-dropdown-content {
  right: 0;
  border-top-right-radius: 0px;
}
.menu-item-dropdown-center .menu-dropdown-content,
.menu-dropdown-center .menu-dropdown-content {
  left: 50%;
  min-width: calc(100% + 24px + 24px);
  transform: translateX(-50%);
}
/* === Color Picker === */
:root {
  --f7-color-picker-popover-width: 350px;
  --f7-color-picker-slider-size: 6px;
  --f7-color-picker-slider-knob-size: 16px;
  --f7-color-picker-bar-size: 50px;
  --f7-color-picker-bar-min-height: 260px;
  --f7-color-picker-value-width: 64px;
  --f7-color-picker-value-height: 32px;
  --f7-color-picker-value-font-size: 16px;
  --f7-color-picker-value-border-radius: 4px;
  --f7-color-picker-hex-value-width: 84px;
  --f7-color-picker-label-font-size: 14px;
  --f7-color-picker-label-width: 10px;
  --f7-color-picker-label-height: 14px;
  --f7-color-picker-sb-spectrum-height: 260px;
  --f7-color-picker-sb-spectrum-handle-size: 16px;
  --f7-color-picker-wheel-width: 330px;
  --f7-color-picker-palette-value-width: 36px;
  --f7-color-picker-palette-value-height: 36px;
  --f7-color-picker-initial-current-color-height: 40px;
  --f7-color-picker-initial-current-color-border-radius: 4px;
  --f7-color-picker-sheet-bg-color: #fff;
  --f7-color-picker-popup-bg-color: #fff;
  --f7-color-picker-value-bg-color: rgba(0, 0, 0, 0.05);
  --f7-color-picker-group-bg-color: rgba(0, 0, 0, 0.05);
  --f7-color-picker-group-value-bg-color: #fff;
}
:root .theme-dark,
:root.theme-dark {
  --f7-color-picker-sheet-bg-color: #121212;
  --f7-color-picker-popup-bg-color: #121212;
  --f7-color-picker-value-bg-color: rgba(255, 255, 255, 0.1);
  --f7-color-picker-group-bg-color: #000;
  --f7-color-picker-group-value-bg-color: rgba(255, 255, 255, 0.12);
}
.color-picker {
  overflow: hidden;
  width: 100%;
  display: flex;
  flex-direction: column;
}
.color-picker.color-picker-inline,
.color-picker-popover .color-picker,
.color-picker-popup .color-picker {
  position: relative;
}
.color-picker-sheet-modal {
  background: var(--f7-color-picker-sheet-bg-color);
}
.color-picker-sheet-modal:before {
  z-index: 600;
}
.color-picker-sheet-modal .sheet-modal-inner {
  margin-bottom: var(--f7-safe-area-bottom);
}
.color-picker-popup .page {
  background: var(--f7-color-picker-popup-bg-color);
}
.color-picker-popup .page-content {
  padding-bottom: var(--f7-safe-area-bottom);
}
.color-picker-popover .color-picker,
.color-picker-popup .color-picker,
.color-picker-page .color-picker {
  height: 100%;
}
.color-picker-popover .color-picker .toolbar,
.color-picker-popup .color-picker .toolbar,
.color-picker-page .color-picker .toolbar {
  position: absolute;
}
.color-picker-popover {
  width: var(--f7-color-picker-popover-width);
  max-width: 90vw;
  max-height: 80vh;
}
.color-picker-popover .color-picker {
  max-height: 80vh;
}
.color-picker-popover .toolbar-top {
  border-top-left-radius: var(--f7-popover-border-radius);
  border-top-right-radius: var(--f7-popover-border-radius);
}
.color-picker-popover .color-picker-module-palette {
  overflow: hidden;
  flex-shrink: 0;
}
.color-picker-popover .color-picker-module-palette:first-child {
  border-top-left-radius: var(--f7-popover-border-radius);
  border-top-right-radius: var(--f7-popover-border-radius);
}
.color-picker-popover .color-picker-module-palette:last-child {
  border-bottom-left-radius: var(--f7-popover-border-radius);
  border-bottom-right-radius: var(--f7-popover-border-radius);
}
.color-picker-popover .color-picker-module-palette:first-child:last-child {
  border-radius: var(--f7-popover-border-radius);
}
.color-picker-popover .toolbar ~ .page-content .color-picker-module-palette:first-child {
  border-top-left-radius: 0;
  border-top-right-radius: 0;
}
.color-picker-popup .page-content,
.color-picker-popover .page-content,
.color-picker-sheet-modal .page-content,
.color-picker-page .page-content {
  display: flex;
  justify-content: flex-start;
  align-items: stretch;
  flex-direction: column;
  overflow-x: hidden;
}
.color-picker-module {
  margin-top: 5px;
}
.color-picker-module:last-child {
  margin-bottom: 5px;
}
.color-picker-module-sb-spectrum,
.color-picker-module-hs-spectrum {
  margin-left: 10px;
  margin-right: 10px;
}
.color-picker-module-sb-spectrum:first-child,
.color-picker-module-hs-spectrum:first-child {
  margin-top: 10px;
}
.color-picker-module-sb-spectrum .color-picker-sb-spectrum,
.color-picker-module-hs-spectrum .color-picker-sb-spectrum,
.color-picker-module-sb-spectrum .color-picker-hs-spectrum,
.color-picker-module-hs-spectrum .color-picker-hs-spectrum {
  border-radius: 4px;
  height: var(--f7-color-picker-sb-spectrum-height);
}
.color-picker-sb-spectrum {
  background-color: #000;
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0) 0%, #000 100%), linear-gradient(to left, rgba(255, 255, 255, 0) 0%, #fff 100%);
  position: relative;
}
.color-picker-hs-spectrum {
  position: relative;
  background-image: linear-gradient(to right, hsl(0, 100%, 50%), hsl(60, 100%, 50%), hsl(120, 100%, 50%), hsl(180, 100%, 50%), hsl(240, 100%, 50%), hsl(300, 100%, 50%), hsl(0, 100%, 50%));
}
.color-picker-hs-spectrum:after {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0), #ffffff);
}
.color-picker-sb-spectrum-handle,
.color-picker-hs-spectrum-handle {
  width: 4px;
  height: 4px;
  position: absolute;
  left: -2px;
  top: -2px;
  z-index: 1;
}
.color-picker-sb-spectrum-handle:after,
.color-picker-hs-spectrum-handle:after {
  background-color: inherit;
  content: '';
  position: absolute;
  width: var(--f7-color-picker-sb-spectrum-handle-size);
  height: var(--f7-color-picker-sb-spectrum-handle-size);
  border: 1px solid #fff;
  border-radius: 50%;
  box-shadow: 0px 0px 2px rgba(0, 0, 0, 0.5);
  box-sizing: border-box;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  transition: 150ms;
  transition-property: transform;
  transform-origin: center;
}
.color-picker-sb-spectrum-handle.color-picker-sb-spectrum-handle-pressed:after,
.color-picker-hs-spectrum-handle.color-picker-sb-spectrum-handle-pressed:after,
.color-picker-sb-spectrum-handle.color-picker-hs-spectrum-handle-pressed:after,
.color-picker-hs-spectrum-handle.color-picker-hs-spectrum-handle-pressed:after {
  transform: scale(1.5) translate(-33.333%, -33.333%);
}
.color-picker-module-wheel {
  margin-left: 10px;
  margin-right: 10px;
}
.color-picker-wheel {
  position: relative;
  width: var(--f7-color-picker-wheel-width);
  max-width: 100%;
  height: auto;
  font-size: 0;
  margin-left: auto;
  margin-right: auto;
}
.color-picker-wheel svg {
  width: 100%;
  height: auto;
}
.color-picker-wheel .color-picker-wheel-handle {
  width: calc(100% / 6);
  height: calc(100% / 6);
  position: absolute;
  box-sizing: border-box;
  border: 2px solid #fff;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.5);
  background: red;
  border-radius: 50%;
  left: 0;
  top: 0;
}
.color-picker-wheel .color-picker-sb-spectrum {
  width: 45%;
  height: 45%;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
  position: absolute;
}
.color-picker-slider-wrap {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}
.color-picker-slider-wrap + .color-picker-slider-wrap {
  margin-top: 5px;
}
.color-picker-hex-wrap {
  justify-content: space-between;
  display: flex;
  align-items: center;
}
.color-picker-slider-label,
.color-picker-hex-label {
  font-size: var(--f7-color-picker-label-font-size);
  width: var(--f7-color-picker-label-size);
  flex-shrink: 0;
  margin-right: 12px;
}
.color-picker-hex-label {
  width: auto;
}
.color-picker-bar-value,
.color-picker-slider-value,
.color-picker-hex-value {
  width: var(--f7-color-picker-value-width);
  height: var(--f7-color-picker-value-height);
  background: var(--f7-color-picker-value-bg-color);
  border-radius: var(--f7-color-picker-value-border-radius);
  text-align: center;
  font-size: var(--f7-color-picker-value-font-size);
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  margin-left: 10px;
}
.color-picker-bar-value input,
.color-picker-slider-value input,
.color-picker-hex-value input {
  width: 100%;
  height: 100%;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  border: none;
  outline: 0;
  background: transparent;
  color: inherit;
  font-family: inherit;
  font-size: inherit;
  text-align: center;
  display: block;
  border-radius: 4px;
}
.color-picker-bar-value input::-webkit-inner-spin-button,
.color-picker-slider-value input::-webkit-inner-spin-button,
.color-picker-hex-value input::-webkit-inner-spin-button,
.color-picker-bar-value input::-webkit-outer-spin-button,
.color-picker-slider-value input::-webkit-outer-spin-button,
.color-picker-hex-value input::-webkit-outer-spin-button {
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  margin: 0;
  display: none;
}
.color-picker-hex-value {
  width: var(--f7-color-picker-hex-value-width);
}
.color-picker-hex-value:first-child {
  margin-left: auto;
}
.color-picker-slider {
  --f7-range-bar-active-bg-color: transparent;
  --f7-range-bar-size: var(--f7-color-picker-slider-size);
  --f7-range-bar-border-radius: var(--f7-color-picker-slider-size);
  --f7-range-knob-size: var(--f7-color-picker-slider-knob-size);
  --f7-range-knob-box-shadow: 0 1px 2px rgba(0, 0, 0, 0.3);
}
.color-picker-slider .range-knob {
  transition-duration: 200ms;
  transition-property: transform;
}
.color-picker-slider .range-knob:after {
  width: 30px;
  height: 30px;
  margin-left: -16px;
  margin-top: -16px;
}
.color-picker-slider .range-knob-active-state .range-knob {
  transform: scale(1.5);
}
.md .color-picker-slider.range-slider-min:not(.range-slider-dual) .range-knob {
  background: var(--f7-range-knob-color) !important;
  border: none;
}
.color-picker-module-rgb-bars {
  display: flex;
  justify-content: space-around;
  justify-content: space-evenly;
  align-items: stretch;
  height: 100%;
  min-height: var(--f7-color-picker-bar-min-height);
  padding-bottom: 10px;
  padding-top: 10px;
  box-sizing: border-box;
}
.color-picker-bar-wrap {
  display: flex;
  align-items: center;
  flex-direction: column-reverse;
}
.color-picker-bar {
  --f7-range-bar-active-bg-color: transparent;
  --f7-range-bar-size: var(--f7-color-picker-bar-size);
  --f7-range-bar-border-radius: 2px;
  --f7-range-knob-size: 6px;
  --f7-range-knob-box-shadow: 0 0px 3px rgba(0, 0, 0, 0.3);
  --f7-range-knob-color: #fff;
}
.color-picker-bar .range-knob {
  transition-duration: 0ms;
  transition-property: transform;
  border-radius: 3px;
}
.color-picker-bar .range-knob-wrap {
  height: 6px;
  width: calc(var(--f7-color-picker-bar-size) - 4px);
  margin-left: calc(-0.5 * (var(--f7-color-picker-bar-size) - 4px));
}
.color-picker-bar .range-knob-active-state .range-knob {
  transform: scale(1);
}
.md .color-picker-bar.range-slider-min:not(.range-slider-dual) .range-knob {
  background: var(--f7-range-knob-color) !important;
  border: none;
}
.color-picker-bar-label {
  font-size: var(--f7-color-picker-label-size);
  margin-top: 12px;
  line-height: 1;
  height: var(--f7-color-picker-label-height);
  flex-shrink: 0;
}
.color-picker-bar-value {
  margin-left: 0;
  margin-bottom: 10px;
}
.color-picker-slider-alpha {
  --f7-range-knob-color: #fff;
}
.color-picker-slider-alpha .range-bar {
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), #000), linear-gradient(to right, rgba(255, 255, 255, 0.2) 50%, rgba(0, 0, 0, 0.2) 50%), linear-gradient(to left, rgba(255, 255, 255, 0.2) 50%, rgba(0, 0, 0, 0.2) 50%);
  background-size: 100% 100%, 6px 3px, 6px 3px;
  background-position: 0 0, 0px 3px, 0 0;
  background-repeat: repeat-y, repeat-x, repeat-x;
}
.color-picker-slider-hue .range-bar {
  background-image: linear-gradient(to right, hsl(0, 100%, 50%), hsl(60, 100%, 50%), hsl(120, 100%, 50%), hsl(180, 100%, 50%), hsl(240, 100%, 50%), hsl(300, 100%, 50%), hsl(0, 100%, 50%));
}
.color-picker-slider-brightness .range-bar {
  background-image: linear-gradient(to right, #000, #fff);
}
.color-picker-module-palette {
  margin-top: 16px;
}
.color-picker-module-palette:first-child {
  margin-top: 0;
}
.color-picker-module-palette:last-child {
  margin-bottom: 0;
}
.color-picker-module-palette:first-child:last-child {
  margin: 0;
}
.color-picker-palette {
  display: flex;
  flex-wrap: wrap;
}
.color-picker-palette-row {
  width: 100%;
  display: flex;
  flex-wrap: nowrap;
}
.color-picker-palette-row .color-picker-palette-value {
  width: 100%;
}
.color-picker-palette-value {
  width: var(--f7-color-picker-palette-value-width);
  height: var(--f7-color-picker-palette-value-height);
  cursor: pointer;
}
.color-picker-module-initial-current-colors,
.color-picker-module-current-color {
  margin-left: 10px;
  margin-right: 10px;
  border-radius: var(--f7-color-picker-initial-current-color-border-radius);
  overflow: hidden;
  flex-shrink: 0;
}
.color-picker-initial-color,
.color-picker-current-color {
  height: var(--f7-color-picker-initial-current-color-height);
}
.color-picker-initial-current-colors {
  display: flex;
}
.color-picker-initial-current-colors .color-picker-initial-color,
.color-picker-initial-current-colors .color-picker-current-color {
  width: 50%;
}
.color-picker-module-rgb-sliders,
.color-picker-module-hsb-sliders,
.color-picker-module-alpha-slider,
.color-picker-module-hue-slider,
.color-picker-module-brightness-slider,
.color-picker-module-hex {
  margin-left: 10px;
  margin-right: 10px;
}
.color-picker-grouped-modules .color-picker-module-rgb-sliders,
.color-picker-grouped-modules .color-picker-module-hsb-sliders,
.color-picker-grouped-modules .color-picker-module-alpha-slider,
.color-picker-grouped-modules .color-picker-module-hue-slider,
.color-picker-grouped-modules .color-picker-module-brightness-slider,
.color-picker-grouped-modules .color-picker-module-hex {
  background: var(--f7-color-picker-group-bg-color);
  padding: 5px;
  border-radius: 4px;
  margin-top: 16px;
  margin-left: 5px;
  margin-right: 5px;
}
.color-picker-grouped-modules .color-picker-module-rgb-sliders:last-child,
.color-picker-grouped-modules .color-picker-module-hsb-sliders:last-child,
.color-picker-grouped-modules .color-picker-module-alpha-slider:last-child,
.color-picker-grouped-modules .color-picker-module-hue-slider:last-child,
.color-picker-grouped-modules .color-picker-module-brightness-slider:last-child,
.color-picker-grouped-modules .color-picker-module-hex:last-child {
  margin-bottom: 16px;
}
.color-picker-grouped-modules .color-picker-slider-value,
.color-picker-grouped-modules .color-picker-hex-value {
  background: var(--f7-color-picker-group-value-bg-color);
}
.color-picker-grouped-modules .color-picker-slider-label,
.color-picker-grouped-modules .color-picker-hex-label {
  margin-left: 5px;
}
.color-picker-grouped-modules .color-picker-module-rgb-sliders .range-slider:first-child,
.color-picker-grouped-modules .color-picker-module-hsb-sliders .range-slider:first-child,
.color-picker-grouped-modules .color-picker-module-alpha-slider .range-slider:first-child,
.color-picker-grouped-modules .color-picker-module-hue-slider .range-slider:first-child,
.color-picker-grouped-modules .color-picker-module-brightness-slider .range-slider:first-child {
  margin-left: 5px;
}
.color-picker-grouped-modules .color-picker-module-rgb-sliders .range-slider:last-child,
.color-picker-grouped-modules .color-picker-module-hsb-sliders .range-slider:last-child,
.color-picker-grouped-modules .color-picker-module-alpha-slider .range-slider:last-child,
.color-picker-grouped-modules .color-picker-module-hue-slider .range-slider:last-child,
.color-picker-grouped-modules .color-picker-module-brightness-slider .range-slider:last-child {
  margin-right: 5px;
}
/* === Treeview === */
:root {
  --f7-treeview-item-padding-left: 16px;
  --f7-treeview-item-padding-right: 16px;
  --f7-treeview-toggle-size: 24px;
  --f7-treeview-children-offset: 29px;
  --f7-treeview-label-font-weight: 400;
  --f7-treeview-label-text-color: inherit;
  /*
  --f7-treeview-selectable-selected-bg-color: rgba(var(--f7-theme-color-rgb), 0.2);
  */
  --f7-treeview-toggle-color: rgba(0, 0, 0, 0.5);
  --f7-treeview-toggle-hover-bg-color: rgba(0, 0, 0, 0.1);
  --f7-treeview-toggle-pressed-bg-color: rgba(0, 0, 0, 0.15);
  --f7-treeview-icon-color: rgba(0, 0, 0, 0.5);
  --f7-treeview-selectable-hover-bg-color: rgba(0, 0, 0, 0.1);
  --f7-treeview-link-hover-bg-color: rgba(0, 0, 0, 0.1);
  --f7-treeview-link-pressed-bg-color: rgba(0, 0, 0, 0.15);
}
:root .theme-dark,
:root.theme-dark {
  --f7-treeview-toggle-color: rgba(255, 255, 255, 0.5);
  --f7-treeview-toggle-hover-bg-color: rgba(255, 255, 255, 0.03);
  --f7-treeview-toggle-pressed-bg-color: rgba(255, 255, 255, 0.1);
  --f7-treeview-icon-color: rgba(255, 255, 255, 0.75);
  --f7-treeview-selectable-hover-bg-color: rgba(255, 255, 255, 0.03);
  --f7-treeview-link-hover-bg-color: rgba(255, 255, 255, 0.03);
  --f7-treeview-link-pressed-bg-color: rgba(255, 255, 255, 0.11);
}
.ios {
  --f7-treeview-item-height: 34px;
  --f7-treeview-label-font-size: 17px;
  --f7-treeview-icon-size: 24px;
}
.md {
  --f7-treeview-item-height: 34px;
  --f7-treeview-label-font-size: 16px;
  --f7-treeview-icon-size: 24px;
}
.aurora {
  --f7-treeview-item-height: 28px;
  --f7-treeview-label-font-size: 14px;
  --f7-treeview-icon-size: 20px;
}
.treeview-item-root {
  padding-left: var(--f7-treeview-item-padding-left);
  padding-right: var(--f7-treeview-item-padding-right);
  height: var(--f7-treeview-item-height);
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
.treeview-item-content {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}
.treeview-item-content > i,
.treeview-item-content > .f7-icons,
.treeview-item-content > .material-icons {
  font-size: var(--f7-treeview-icon-size);
  color: var(--f7-treeview-icon-color);
}
.treeview-item-content:first-child {
  margin-left: calc(var(--f7-treeview-toggle-size) + 5px);
}
.treeview-item-content > * + * {
  margin-left: 5px;
}
.treeview-item-label {
  font-size: var(--f7-treeview-label-font-size);
  font-weight: var(--f7-treeview-label-font-weight);
  color: var(--f7-treeview-label-text-color);
}
.treeview-toggle {
  width: var(--f7-treeview-toggle-size);
  height: var(--f7-treeview-toggle-size);
  cursor: pointer;
  border-radius: 4px;
  background-color: rgba(0, 0, 0, 0);
  transition-duration: 200ms;
  position: relative;
  margin-right: 5px;
}
.treeview-toggle.active-state {
  background-color: var(--f7-treeview-toggle-pressed-bg-color);
}
.treeview-toggle:after {
  transition-duration: 200ms;
  content: '';
  position: absolute;
  left: 50%;
  top: 50%;
  width: 0;
  height: 0;
  border-top: 5px solid transparent;
  border-bottom: 5px solid transparent;
  transform: translate(-50%, -50%);
  border-left: 6px solid var(--f7-treeview-toggle-color);
}
.treeview-toggle-hidden {
  opacity: 0;
  pointer-events: none;
  visibility: hidden;
}
.treeview-preloader {
  --f7-preloader-size: var(--f7-treeview-toggle-size);
  margin-right: calc(-1 * var(--f7-treeview-toggle-size));
}
.treeview-item-children {
  display: none;
}
.treeview-item-opened > .treeview-item-children {
  display: block;
}
.treeview-item-opened > .treeview-item-root .treeview-toggle:after {
  transform: translate(-50%, -50%) rotate(90deg);
}
a.treeview-item-root {
  color: var(--f7-treeview-label-text-color);
}
.treeview-item-selectable > .treeview-item-root,
.treeview-item-selectable.treeview-item-root {
  cursor: pointer;
  transition-duration: 150ms;
}
a.treeview-item-root {
  transition-duration: 150ms;
}
a.treeview-item-root.active-state {
  background: var(--f7-treeview-link-pressed-bg-color);
}
.treeview-item-toggle > .treeview-item-root,
.treeview-item-toggle.treeview-item-root {
  cursor: pointer;
}
.treeview-item-selected > .treeview-item-root,
.treeview-item-selected.treeview-item-root {
  background: var(--f7-treeview-selectable-selected-bg-color, rgba(var(--f7-theme-color-rgb), 0.2));
}
.treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 1);
}
.treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 2);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 3);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 4);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 5);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 6);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 7);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 8);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 9);
}
.treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item .treeview-item-root {
  padding-left: calc(var(--f7-treeview-item-padding-left) + var(--f7-treeview-children-offset) * 10);
}
.aurora .treeview-toggle:hover {
  background-color: var(--f7-treeview-toggle-hover-bg-color);
}
.aurora .treeview-toggle.active-state {
  background-color: var(--f7-treeview-toggle-pressed-bg-color);
}
.aurora .treeview-item-selectable > .treeview-item-root:hover,
.aurora .treeview-item-selectable.treeview-item-root:hover {
  background: var(--f7-treeview-selectable-hover-bg-color);
}
.aurora a.treeview-item-root:hover {
  background: var(--f7-treeview-link-hover-bg-color);
}
.aurora a.treeview-item-root.active-state {
  background: var(--f7-treeview-link-pressed-bg-color);
}
.aurora .treeview-item-selected > .treeview-item-root:hover,
.aurora .treeview-item-selected.treeview-item-root:hover {
  background: var(--f7-treeview-selectable-selected-bg-color, rgba(var(--f7-theme-color-rgb), 0.2));
}
/* === Stepper === */
:root {
  --f7-text-editor-font-size: inherit;
  --f7-text-editor-font-weight: inherit;
  --f7-text-editor-border-width: 1px;
  --f7-text-editor-height: 250px;
  --f7-text-editor-margin: 16px;
  --f7-text-editor-padding: 8px;
  --f7-text-editor-button-bg-color: transparent;
  --f7-text-editor-button-size: 28px;
  --f7-text-editor-button-icon-size: 20px;
  --f7-text-editor-button-margin: 2px;
  --f7-text-editor-button-border-radius: 2px;
  --f7-text-editor-text-color: #000;
  --f7-text-editor-bg-color: #fff;
  --f7-text-editor-border-color: rgba(0, 0, 0, 0.1);
  --f7-text-editor-toolbar-bg-color: #fff;
  --f7-text-editor-button-text-color: #333;
  --f7-text-editor-button-divider-color: rgba(0, 0, 0, 0.15);
  --f7-text-editor-placeholder-color: rgba(0, 0, 0, 0.35);
}
:root .theme-dark,
:root.theme-dark {
  --f7-text-editor-bg-color: #121212;
  --f7-text-editor-border-color: rgba(255, 255, 255, 0.1);
  --f7-text-editor-toolbar-bg-color: #202020;
  --f7-text-editor-text-color: #fff;
  --f7-text-editor-placeholder-color: rgba(255, 255, 255, 0.35);
  --f7-text-editor-button-text-color: #fff;
  --f7-text-editor-button-divider-color: rgba(255, 255, 255, 0.15);
}
.ios {
  --f7-text-editor-toolbar-padding: 6px;
  --f7-text-editor-toolbar-border-color: rgba(0, 0, 0, 0.25);
}
.ios .theme-dark,
.ios.theme-dark {
  --f7-text-editor-toolbar-bg-color: #121212;
  --f7-text-editor-toolbar-border-color: rgba(255, 255, 255, 0.1);
}
.md {
  --f7-text-editor-toolbar-padding: 8px;
  --f7-text-editor-toolbar-box-shadow: 0px 2px 3px -1px rgba(0, 0, 0, 0.25);
}
.aurora {
  --f7-text-editor-toolbar-padding: 3px;
  --f7-text-editor-toolbar-border-color: rgba(0, 0, 0, 0.25);
}
.aurora .theme-dark,
.aurora.theme-dark {
  --f7-text-editor-toolbar-border-color: rgba(255, 255, 255, 0.1);
}
.text-editor {
  margin: var(--f7-text-editor-margin);
  background-color: var(--f7-text-editor-bg-color);
  display: block;
  position: relative;
  border: var(--f7-text-editor-border-width) solid var(--f7-text-editor-border-color);
  display: flex;
  flex-direction: column;
  align-items: stretch;
  height: var(--f7-text-editor-height);
  box-sizing: border-box;
}
.text-editor.text-editor-resizable {
  height: auto;
}
.text-editor-toolbar {
  display: flex;
  flex-wrap: wrap;
  background: var(--f7-text-editor-toolbar-bg-color);
  z-index: 100;
  position: relative;
  position: -webkit-sticky;
  position: sticky;
  left: 0;
  top: 0;
  padding: var(--f7-text-editor-toolbar-padding);
  flex-shrink: 0;
  box-shadow: var(--f7-text-editor-toolbar-box-shadow);
  box-sizing: border-box;
}
.text-editor-toolbar:after {
  content: '';
  position: absolute;
  background-color: var(--f7-text-editor-toolbar-border-color);
  display: block;
  z-index: 15;
  top: auto;
  right: auto;
  bottom: 0;
  left: 0;
  height: 1px;
  width: 100%;
  transform-origin: 50% 100%;
  transform: scaleY(calc(1 / var(--f7-device-pixel-ratio)));
}
button.text-editor-button {
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  border: none;
  padding: 0;
  margin: 0;
  outline: 0;
  font-family: inherit;
  background: transparent;
  cursor: pointer;
  box-shadow: none;
  border-radius: var(--f7-text-editor-button-border-radius);
  position: relative;
  z-index: 1;
  display: flex;
  width: auto;
  overflow: hidden;
  width: var(--f7-text-editor-button-size);
  height: var(--f7-text-editor-button-size);
  align-items: center;
  justify-content: center;
  margin: var(--f7-text-editor-button-margin);
  box-sizing: border-box;
  color: var(--f7-text-editor-button-text-color);
  background-color: var(--f7-text-editor-button-bg-color);
  flex-shrink: 0;
}
button.text-editor-button i {
  font-size: var(--f7-text-editor-button-icon-size);
  font-style: normal;
}
button.text-editor-button i sup,
button.text-editor-button i sub {
  font-size: 60%;
}
.text-editor-button-divider {
  width: 1px;
  background: var(--f7-text-editor-button-divider-color);
  margin: 0 2px;
  flex-shrink: 0;
}
.text-editor-content {
  -webkit-user-modify: read-write;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  border: none;
  outline: 0;
  height: 100%;
  -webkit-user-select: text;
     -moz-user-select: text;
          user-select: text;
  padding: var(--f7-text-editor-padding);
  overflow: auto;
  flex-shrink: 10;
  box-sizing: border-box;
  color: var(--f7-text-editor-text-color);
  font-size: var(--f7-text-editor-font-size);
  font-weight: var(--f7-text-editor-font-weight);
}
.text-editor-content .text-editor-placeholder {
  pointer-events: none;
  color: var(--f7-text-editor-placeholder-color);
}
.text-editor-content img {
  max-width: 100%;
}
.text-editor-content a {
  pointer-events: none;
}
.text-editor-popover {
  z-index: 12500;
  width: auto;
  max-width: 80vw;
}
.text-editor-popover .popover-inner {
  display: flex;
  flex-wrap: wrap;
  padding: 3px;
}
.text-editor-keyboard-toolbar {
  position: absolute;
  z-index: 6000;
  --f7-safe-area-bottom: 0px;
}
.text-editor-keyboard-toolbar .toolbar-inner {
  justify-content: flex-start !important;
  overflow: auto;
  -webkit-overflow-scrolling: touch;
}
.text-editor-keyboard-toolbar .toolbar-inner::-webkit-scrollbar {
  display: none;
}
.text-editor-keyboard-toolbar .toolbar-inner .text-editor-button-divider {
  height: 100%;
}
.item-input .text-editor {
  border: none;
  margin: 0;
  background-color: var(--f7-input-bg-color, transparent);
}
.item-input .text-editor-content {
  padding-top: var(--f7-textarea-padding-vertical);
  padding-bottom: var(--f7-textarea-padding-vertical);
  padding-left: var(--f7-input-padding-left);
  padding-right: var(--f7-input-padding-right);
  color: var(--f7-input-text-color);
  font-size: var(--f7-input-font-size);
}
.item-input .text-editor-toolbar {
  box-shadow: none;
}
.item-input .text-editor-toolbar:after {
  display: none !important;
}
.item-input-outline .text-editor-content {
  border-radius: var(--f7-input-outline-border-radius);
  padding-left: var(--f7-input-outline-padding-horizontal);
  padding-right: var(--f7-input-outline-padding-horizontal);
}
.ios button.text-editor-button {
  transition: opacity 300ms;
}
.ios button.text-editor-button.active-state {
  opacity: 0.3;
  transition-duration: 0ms;
}
.md button.text-editor-button:before {
  content: '';
  width: 152%;
  height: 152%;
  position: absolute;
  left: -26%;
  top: -26%;
  background-image: radial-gradient(circle at center, var(--f7-link-highlight-color) 66%, rgba(255, 255, 255, 0) 66%);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%;
  opacity: 0;
  pointer-events: none;
  transition-duration: 600ms;
}
.md button.text-editor-button.active-state:before {
  opacity: 1;
  transition-duration: 150ms;
}
.md .text-editor-keyboard-toolbar .toolbar-inner {
  padding-left: 8px;
  padding-right: 8px;
}
.aurora button.text-editor-button {
  transition: opacity 300ms;
}
.aurora button.text-editor-button.active-state {
  opacity: 0.3;
  transition-duration: 0ms;
}
/* === Elevation === */
:root {
  --f7-elevation-0: 0px 0px 0px 0px rgba(0, 0, 0, 0);
  --f7-elevation-1: 0px 2px 1px -1px rgba(0, 0, 0, 0.2),
    0px 1px 1px 0px rgba(0, 0, 0, 0.14),
    0px 1px 3px 0px rgba(0, 0, 0, 0.12);
  --f7-elevation-2: 0px 3px 1px -2px rgba(0, 0, 0, 0.2),
    0px 2px 2px 0px rgba(0, 0, 0, 0.14),
    0px 1px 5px 0px rgba(0, 0, 0, 0.12);
  --f7-elevation-3: 0px 3px 3px -2px rgba(0, 0, 0, 0.2),
    0px 3px 4px 0px rgba(0, 0, 0, 0.14),
    0px 1px 8px 0px rgba(0, 0, 0, 0.12);
  --f7-elevation-4: 0px 2px 4px -1px rgba(0, 0, 0, 0.2),
    0px 4px 5px 0px rgba(0, 0, 0, 0.14),
    0px 1px 10px 0px rgba(0, 0, 0, 0.12);
  --f7-elevation-5: 0px 3px 5px -1px rgba(0, 0, 0, 0.2),
    0px 5px 8px 0px rgba(0, 0, 0, 0.14),
    0px 1px 14px 0px rgba(0, 0, 0, 0.12);
  --f7-elevation-6: 0px 3px 5px -1px rgba(0, 0, 0, 0.2),
    0px 6px 10px 0px rgba(0, 0, 0, 0.14),
    0px 1px 18px 0px rgba(0, 0, 0, 0.12);
  --f7-elevation-7: 0px 4px 5px -2px rgba(0, 0, 0, 0.2),
    0px 7px 10px 1px rgba(0, 0, 0, 0.14),
    0px 2px 16px 1px rgba(0, 0, 0, 0.12);
  --f7-elevation-8: 0px 5px 5px -3px rgba(0, 0, 0, 0.2),
    0px 8px 10px 1px rgba(0, 0, 0, 0.14),
    0px 3px 14px 2px rgba(0, 0, 0, 0.12);
  --f7-elevation-9: 0px 5px 6px -3px rgba(0, 0, 0, 0.2),
    0px 9px 12px 1px rgba(0, 0, 0, 0.14),
    0px 3px 16px 2px rgba(0, 0, 0, 0.12);
  --f7-elevation-10: 0px 6px 6px -3px rgba(0, 0, 0, 0.2),
    0px 10px 14px 1px rgba(0, 0, 0, 0.14),
    0px 4px 18px 3px rgba(0, 0, 0, 0.12);
  --f7-elevation-11: 0px 6px 7px -4px rgba(0, 0, 0, 0.2),
    0px 11px 15px 1px rgba(0, 0, 0, 0.14),
    0px 4px 20px 3px rgba(0, 0, 0, 0.12);
  --f7-elevation-12: 0px 7px 8px -4px rgba(0, 0, 0, 0.2),
    0px 12px 17px 2px rgba(0, 0, 0, 0.14),
    0px 5px 22px 4px rgba(0, 0, 0, 0.12);
  --f7-elevation-13: 0px 7px 8px -4px rgba(0, 0, 0, 0.2),
    0px 13px 19px 2px rgba(0, 0, 0, 0.14),
    0px 5px 24px 4px rgba(0, 0, 0, 0.12);
  --f7-elevation-14: 0px 7px 9px -4px rgba(0, 0, 0, 0.2),
    0px 14px 21px 2px rgba(0, 0, 0, 0.14),
    0px 5px 26px 4px rgba(0, 0, 0, 0.12);
  --f7-elevation-15: 0px 8px 9px -5px rgba(0, 0, 0, 0.2),
    0px 15px 22px 2px rgba(0, 0, 0, 0.14),
    0px 6px 28px 5px rgba(0, 0, 0, 0.12);
  --f7-elevation-16: 0px 8px 10px -5px rgba(0, 0, 0, 0.2),
    0px 16px 24px 2px rgba(0, 0, 0, 0.14),
    0px 6px 30px 5px rgba(0, 0, 0, 0.12);
  --f7-elevation-17: 0px 8px 11px -5px rgba(0, 0, 0, 0.2),
    0px 17px 26px 2px rgba(0, 0, 0, 0.14),
    0px 6px 32px 5px rgba(0, 0, 0, 0.12);
  --f7-elevation-18: 0px 9px 11px -5px rgba(0, 0, 0, 0.2),
    0px 18px 28px 2px rgba(0, 0, 0, 0.14),
    0px 7px 34px 6px rgba(0, 0, 0, 0.12);
  --f7-elevation-19: 0px 9px 12px -6px rgba(0, 0, 0, 0.2),
    0px 19px 29px 2px rgba(0, 0, 0, 0.14),
    0px 7px 36px 6px rgba(0, 0, 0, 0.12);
  --f7-elevation-20: 0px 10px 13px -6px rgba(0, 0, 0, 0.2),
    0px 20px 31px 3px rgba(0, 0, 0, 0.14),
    0px 8px 38px 7px rgba(0, 0, 0, 0.12);
  --f7-elevation-21: 0px 10px 13px -6px rgba(0, 0, 0, 0.2),
    0px 21px 33px 3px rgba(0, 0, 0, 0.14),
    0px 8px 40px 7px rgba(0, 0, 0, 0.12);
  --f7-elevation-22: 0px 10px 14px -6px rgba(0, 0, 0, 0.2),
    0px 22px 35px 3px rgba(0, 0, 0, 0.14),
    0px 8px 42px 7px rgba(0, 0, 0, 0.12);
  --f7-elevation-23: 0px 11px 14px -7px rgba(0, 0, 0, 0.2),
    0px 23px 36px 3px rgba(0, 0, 0, 0.14),
    0px 9px 44px 8px rgba(0, 0, 0, 0.12);
  --f7-elevation-24: 0px 11px 15px -7px rgba(0, 0, 0, 0.2),
    0px 24px 38px 3px rgba(0, 0, 0, 0.14),
    0px 9px 46px 8px rgba(0, 0, 0, 0.12);
}
.elevation-0 {
  box-shadow: var(--f7-elevation-0) !important;
}
.elevation-1 {
  box-shadow: var(--f7-elevation-1) !important;
}
.elevation-2 {
  box-shadow: var(--f7-elevation-2) !important;
}
.elevation-3 {
  box-shadow: var(--f7-elevation-3) !important;
}
.elevation-4 {
  box-shadow: var(--f7-elevation-4) !important;
}
.elevation-5 {
  box-shadow: var(--f7-elevation-5) !important;
}
.elevation-6 {
  box-shadow: var(--f7-elevation-6) !important;
}
.elevation-7 {
  box-shadow: var(--f7-elevation-7) !important;
}
.elevation-8 {
  box-shadow: var(--f7-elevation-8) !important;
}
.elevation-9 {
  box-shadow: var(--f7-elevation-9) !important;
}
.elevation-10 {
  box-shadow: var(--f7-elevation-10) !important;
}
.elevation-11 {
  box-shadow: var(--f7-elevation-11) !important;
}
.elevation-12 {
  box-shadow: var(--f7-elevation-12) !important;
}
.elevation-13 {
  box-shadow: var(--f7-elevation-13) !important;
}
.elevation-14 {
  box-shadow: var(--f7-elevation-14) !important;
}
.elevation-15 {
  box-shadow: var(--f7-elevation-15) !important;
}
.elevation-16 {
  box-shadow: var(--f7-elevation-16) !important;
}
.elevation-17 {
  box-shadow: var(--f7-elevation-17) !important;
}
.elevation-18 {
  box-shadow: var(--f7-elevation-18) !important;
}
.elevation-19 {
  box-shadow: var(--f7-elevation-19) !important;
}
.elevation-20 {
  box-shadow: var(--f7-elevation-20) !important;
}
.elevation-21 {
  box-shadow: var(--f7-elevation-21) !important;
}
.elevation-22 {
  box-shadow: var(--f7-elevation-22) !important;
}
.elevation-23 {
  box-shadow: var(--f7-elevation-23) !important;
}
.elevation-24 {
  box-shadow: var(--f7-elevation-24) !important;
}
.device-desktop .elevation-hover-0:hover {
  box-shadow: var(--f7-elevation-0) !important;
}
.device-desktop .elevation-hover-1:hover {
  box-shadow: var(--f7-elevation-1) !important;
}
.device-desktop .elevation-hover-2:hover {
  box-shadow: var(--f7-elevation-2) !important;
}
.device-desktop .elevation-hover-3:hover {
  box-shadow: var(--f7-elevation-3) !important;
}
.device-desktop .elevation-hover-4:hover {
  box-shadow: var(--f7-elevation-4) !important;
}
.device-desktop .elevation-hover-5:hover {
  box-shadow: var(--f7-elevation-5) !important;
}
.device-desktop .elevation-hover-6:hover {
  box-shadow: var(--f7-elevation-6) !important;
}
.device-desktop .elevation-hover-7:hover {
  box-shadow: var(--f7-elevation-7) !important;
}
.device-desktop .elevation-hover-8:hover {
  box-shadow: var(--f7-elevation-8) !important;
}
.device-desktop .elevation-hover-9:hover {
  box-shadow: var(--f7-elevation-9) !important;
}
.device-desktop .elevation-hover-10:hover {
  box-shadow: var(--f7-elevation-10) !important;
}
.device-desktop .elevation-hover-11:hover {
  box-shadow: var(--f7-elevation-11) !important;
}
.device-desktop .elevation-hover-12:hover {
  box-shadow: var(--f7-elevation-12) !important;
}
.device-desktop .elevation-hover-13:hover {
  box-shadow: var(--f7-elevation-13) !important;
}
.device-desktop .elevation-hover-14:hover {
  box-shadow: var(--f7-elevation-14) !important;
}
.device-desktop .elevation-hover-15:hover {
  box-shadow: var(--f7-elevation-15) !important;
}
.device-desktop .elevation-hover-16:hover {
  box-shadow: var(--f7-elevation-16) !important;
}
.device-desktop .elevation-hover-17:hover {
  box-shadow: var(--f7-elevation-17) !important;
}
.device-desktop .elevation-hover-18:hover {
  box-shadow: var(--f7-elevation-18) !important;
}
.device-desktop .elevation-hover-19:hover {
  box-shadow: var(--f7-elevation-19) !important;
}
.device-desktop .elevation-hover-20:hover {
  box-shadow: var(--f7-elevation-20) !important;
}
.device-desktop .elevation-hover-21:hover {
  box-shadow: var(--f7-elevation-21) !important;
}
.device-desktop .elevation-hover-22:hover {
  box-shadow: var(--f7-elevation-22) !important;
}
.device-desktop .elevation-hover-23:hover {
  box-shadow: var(--f7-elevation-23) !important;
}
.device-desktop .elevation-hover-24:hover {
  box-shadow: var(--f7-elevation-24) !important;
}
.active-state.elevation-pressed-0,
.device-desktop .active-state.elevation-pressed-0 {
  box-shadow: var(--f7-elevation-0) !important;
}
.active-state.elevation-pressed-1,
.device-desktop .active-state.elevation-pressed-1 {
  box-shadow: var(--f7-elevation-1) !important;
}
.active-state.elevation-pressed-2,
.device-desktop .active-state.elevation-pressed-2 {
  box-shadow: var(--f7-elevation-2) !important;
}
.active-state.elevation-pressed-3,
.device-desktop .active-state.elevation-pressed-3 {
  box-shadow: var(--f7-elevation-3) !important;
}
.active-state.elevation-pressed-4,
.device-desktop .active-state.elevation-pressed-4 {
  box-shadow: var(--f7-elevation-4) !important;
}
.active-state.elevation-pressed-5,
.device-desktop .active-state.elevation-pressed-5 {
  box-shadow: var(--f7-elevation-5) !important;
}
.active-state.elevation-pressed-6,
.device-desktop .active-state.elevation-pressed-6 {
  box-shadow: var(--f7-elevation-6) !important;
}
.active-state.elevation-pressed-7,
.device-desktop .active-state.elevation-pressed-7 {
  box-shadow: var(--f7-elevation-7) !important;
}
.active-state.elevation-pressed-8,
.device-desktop .active-state.elevation-pressed-8 {
  box-shadow: var(--f7-elevation-8) !important;
}
.active-state.elevation-pressed-9,
.device-desktop .active-state.elevation-pressed-9 {
  box-shadow: var(--f7-elevation-9) !important;
}
.active-state.elevation-pressed-10,
.device-desktop .active-state.elevation-pressed-10 {
  box-shadow: var(--f7-elevation-10) !important;
}
.active-state.elevation-pressed-11,
.device-desktop .active-state.elevation-pressed-11 {
  box-shadow: var(--f7-elevation-11) !important;
}
.active-state.elevation-pressed-12,
.device-desktop .active-state.elevation-pressed-12 {
  box-shadow: var(--f7-elevation-12) !important;
}
.active-state.elevation-pressed-13,
.device-desktop .active-state.elevation-pressed-13 {
  box-shadow: var(--f7-elevation-13) !important;
}
.active-state.elevation-pressed-14,
.device-desktop .active-state.elevation-pressed-14 {
  box-shadow: var(--f7-elevation-14) !important;
}
.active-state.elevation-pressed-15,
.device-desktop .active-state.elevation-pressed-15 {
  box-shadow: var(--f7-elevation-15) !important;
}
.active-state.elevation-pressed-16,
.device-desktop .active-state.elevation-pressed-16 {
  box-shadow: var(--f7-elevation-16) !important;
}
.active-state.elevation-pressed-17,
.device-desktop .active-state.elevation-pressed-17 {
  box-shadow: var(--f7-elevation-17) !important;
}
.active-state.elevation-pressed-18,
.device-desktop .active-state.elevation-pressed-18 {
  box-shadow: var(--f7-elevation-18) !important;
}
.active-state.elevation-pressed-19,
.device-desktop .active-state.elevation-pressed-19 {
  box-shadow: var(--f7-elevation-19) !important;
}
.active-state.elevation-pressed-20,
.device-desktop .active-state.elevation-pressed-20 {
  box-shadow: var(--f7-elevation-20) !important;
}
.active-state.elevation-pressed-21,
.device-desktop .active-state.elevation-pressed-21 {
  box-shadow: var(--f7-elevation-21) !important;
}
.active-state.elevation-pressed-22,
.device-desktop .active-state.elevation-pressed-22 {
  box-shadow: var(--f7-elevation-22) !important;
}
.active-state.elevation-pressed-23,
.device-desktop .active-state.elevation-pressed-23 {
  box-shadow: var(--f7-elevation-23) !important;
}
.active-state.elevation-pressed-24,
.device-desktop .active-state.elevation-pressed-24 {
  box-shadow: var(--f7-elevation-24) !important;
}
.elevation-transition-100 {
  transition-duration: 100ms;
  transition-property: box-shadow;
}
.elevation-transition,
.elevation-transition-200 {
  transition-duration: 200ms;
  transition-property: box-shadow;
}
.elevation-transition-300 {
  transition-duration: 300ms;
  transition-property: box-shadow;
}
.elevation-transition-400 {
  transition-duration: 400ms;
  transition-property: box-shadow;
}
.elevation-transition-500 {
  transition-duration: 500ms;
  transition-property: box-shadow;
}
/* === Typography === */
:root {
  --f7-typography-padding: 16px;
  --f7-typography-margin: 16px;
}
.display-flex {
  display: flex !important;
}
.display-block {
  display: block !important;
}
.display-inline-flex {
  display: inline-flex !important;
}
.display-inline-block {
  display: inline-block !important;
}
.display-inline {
  display: inline !important;
}
.display-none {
  display: none !important;
}
.flex-shrink-0 {
  flex-shrink: 0 !important;
}
.flex-shrink-1 {
  flex-shrink: 1 !important;
}
.flex-shrink-2 {
  flex-shrink: 2 !important;
}
.flex-shrink-3 {
  flex-shrink: 3 !important;
}
.flex-shrink-4 {
  flex-shrink: 4 !important;
}
.flex-shrink-5 {
  flex-shrink: 5 !important;
}
.flex-shrink-6 {
  flex-shrink: 6 !important;
}
.flex-shrink-7 {
  flex-shrink: 7 !important;
}
.flex-shrink-8 {
  flex-shrink: 8 !important;
}
.flex-shrink-9 {
  flex-shrink: 9 !important;
}
.flex-shrink-10 {
  flex-shrink: 10 !important;
}
.flex-direction-row {
  flex-direction: row !important;
}
.flex-direction-row-reverse {
  flex-direction: row-reverse !important;
}
.flex-direction-column {
  flex-direction: column !important;
}
.flex-direction-column-reverse {
  flex-direction: column-reverse !important;
}
.justify-content-flex-start {
  justify-content: flex-start !important;
}
.justify-content-center {
  justify-content: center !important;
}
.justify-content-flex-end {
  justify-content: flex-end !important;
}
.justify-content-space-between {
  justify-content: space-between !important;
}
.justify-content-space-around {
  justify-content: space-around !important;
}
.justify-content-space-evenly {
  justify-content: space-evenly !important;
}
.justify-content-stretch {
  justify-content: stretch !important;
}
.justify-content-start {
  justify-content: start !important;
}
.justify-content-end {
  justify-content: end !important;
}
.justify-content-left {
  justify-content: left !important;
}
.justify-content-right {
  justify-content: right !important;
}
.align-content-flex-start {
  align-content: flex-start !important;
}
.align-content-flex-end {
  align-content: flex-end !important;
}
.align-content-center {
  align-content: center !important;
}
.align-content-space-between {
  align-content: space-between !important;
}
.align-content-space-around {
  align-content: space-around !important;
}
.align-content-stretch {
  align-content: stretch !important;
}
.align-items-baseline {
  align-items: baseline !important;
}
.align-items-flex-start {
  align-items: flex-start !important;
}
.align-items-flex-end {
  align-items: flex-end !important;
}
.align-items-center {
  align-items: center !important;
}
.align-items-stretch {
  align-items: stretch !important;
}
.align-self-flex-start {
  align-self: flex-start !important;
}
.align-self-flex-end {
  align-self: flex-end !important;
}
.align-self-center {
  align-self: center !important;
}
.align-self-stretch {
  align-self: stretch !important;
}
.text-align-left {
  text-align: left !important;
}
.text-align-center {
  text-align: center !important;
}
.text-align-right {
  text-align: right !important;
}
.text-align-justify {
  text-align: justify !important;
}
.float-left {
  float: left !important;
}
.float-right {
  float: right !important;
}
.float-none {
  float: none !important;
}
.vertical-align-bottom {
  vertical-align: bottom !important;
}
.vertical-align-middle {
  vertical-align: middle !important;
}
.vertical-align-top {
  vertical-align: top !important;
}
.no-padding {
  padding: 0 !important;
}
.no-padding-left {
  padding-left: 0 !important;
}
.no-padding-right {
  padding-right: 0 !important;
}
.no-padding-horizontal {
  padding-left: 0 !important;
  padding-right: 0 !important;
}
.no-padding-top {
  padding-top: 0 !important;
}
.no-padding-bottom {
  padding-bottom: 0 !important;
}
.no-padding-vertical {
  padding-top: 0 !important;
  padding-bottom: 0 !important;
}
.no-margin {
  margin: 0 !important;
}
.no-margin-left {
  margin-left: 0 !important;
}
.no-margin-right {
  margin-right: 0 !important;
}
.no-margin-horizontal {
  margin-left: 0 !important;
  margin-right: 0 !important;
}
.no-margin-top {
  margin-top: 0 !important;
}
.no-margin-bottom {
  margin-bottom: 0 !important;
}
.no-margin-vertical {
  margin-top: 0 !important;
  margin-bottom: 0 !important;
}
.width-auto {
  width: auto !important;
}
.width-100 {
  width: 100% !important;
}
.padding {
  padding: var(--f7-typography-padding) !important;
}
.padding-half {
  padding: calc(var(--f7-typography-padding) / 2) !important;
}
.padding-top {
  padding-top: var(--f7-typography-padding) !important;
}
.padding-top-half {
  padding-top: calc(var(--f7-typography-padding) / 2) !important;
}
.padding-bottom {
  padding-bottom: var(--f7-typography-padding) !important;
}
.padding-bottom-half {
  padding-bottom: calc(var(--f7-typography-padding) / 2) !important;
}
.padding-left {
  padding-left: var(--f7-typography-padding) !important;
}
.padding-left-half {
  padding-left: calc(var(--f7-typography-padding) / 2) !important;
}
.padding-right {
  padding-right: var(--f7-typography-padding) !important;
}
.padding-right-half {
  padding-right: calc(var(--f7-typography-padding) / 2) !important;
}
.padding-vertical {
  padding-top: var(--f7-typography-padding) !important;
  padding-bottom: var(--f7-typography-padding) !important;
}
.padding-vertical-half {
  padding-top: calc(var(--f7-typography-padding) / 2) !important;
  padding-bottom: calc(var(--f7-typography-padding) / 2) !important;
}
.padding-horizontal {
  padding-left: var(--f7-typography-padding) !important;
  padding-right: var(--f7-typography-padding) !important;
}
.padding-horizontal-half {
  padding-left: calc(var(--f7-typography-padding) / 2) !important;
  padding-right: calc(var(--f7-typography-padding) / 2) !important;
}
.margin {
  margin: var(--f7-typography-margin) !important;
}
.margin-half {
  margin: calc(var(--f7-typography-margin) / 2) !important;
}
.margin-top {
  margin-top: var(--f7-typography-margin) !important;
}
.margin-top-half {
  margin-top: calc(var(--f7-typography-margin) / 2) !important;
}
.margin-bottom {
  margin-bottom: var(--f7-typography-margin) !important;
}
.margin-bottom-half {
  margin-bottom: calc(var(--f7-typography-margin) / 2) !important;
}
.margin-left {
  margin-left: var(--f7-typography-margin) !important;
}
.margin-left-half {
  margin-left: calc(var(--f7-typography-margin) / 2) !important;
}
.margin-right {
  margin-right: var(--f7-typography-margin) !important;
}
.margin-right-half {
  margin-right: calc(var(--f7-typography-margin) / 2) !important;
}
.margin-vertical {
  margin-top: var(--f7-typography-margin) !important;
  margin-bottom: var(--f7-typography-margin) !important;
}
.margin-vertical-half {
  margin-top: calc(var(--f7-typography-margin) / 2) !important;
  margin-bottom: calc(var(--f7-typography-margin) / 2) !important;
}
.margin-horizontal {
  margin-left: var(--f7-typography-margin) !important;
  margin-right: var(--f7-typography-margin) !important;
}
.margin-horizontal-half {
  margin-left: calc(var(--f7-typography-margin) / 2) !important;
  margin-right: calc(var(--f7-typography-margin) / 2) !important;
}
[class*="text-color-"] {
  color: var(--f7-theme-color-text-color) !important;
}
[class*="bg-color-"] {
  background-color: var(--f7-theme-color-bg-color) !important;
}
[class*="border-color-"] {
  border-color: var(--f7-theme-color-border-color) !important;
}
iframe#viAd {
  z-index: 12900 !important;
  background: #000 !important;
}
.vi-overlay {
  background: rgba(0, 0, 0, 0.85);
  z-index: 13100;
  position: absolute;
  left: 0%;
  top: 0%;
  width: 100%;
  height: 100%;
  border-radius: 3px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  align-content: center;
  text-align: center;
  -webkit-user-select: none;
     -moz-user-select: none;
          user-select: none;
}
@supports ((-webkit-backdrop-filter: blur(10px)) or (backdrop-filter: blur(10px))) {
  .vi-overlay {
    background: rgba(0, 0, 0, 0.65);
    -webkit-backdrop-filter: blur(10px);
            backdrop-filter: blur(10px);
  }
}
.vi-overlay .vi-overlay-text {
  text-align: center;
  color: #fff;
  max-width: 80%;
}
.vi-overlay .vi-overlay-text + .vi-overlay-play-button {
  margin-top: 15px;
}
.vi-overlay .vi-overlay-play-button {
  width: 44px;
  height: 44px;
  border-radius: 50%;
  border: 2px solid #fff;
  position: relative;
}
.vi-overlay .vi-overlay-play-button.active-state {
  opacity: 0.55;
}
.vi-overlay .vi-overlay-play-button:before {
  content: '';
  width: 0;
  height: 0;
  border-top: 8px solid transparent;
  border-bottom: 8px solid transparent;
  border-left: 14px solid #fff;
  position: absolute;
  left: 50%;
  top: 50%;
  margin-left: 2px;
  transform: translate(-50%, -50%);
}
