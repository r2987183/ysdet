<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont back-icon">&#xe624;</div>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xe632;</span>
            輸入服務內容
        </div>
        <div class="header-right">
            服務
            <span class="iconfont arrow-icon">&#xe62d;</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HomeHeader'
}
</script>

<!--
1rem = fontsize = 50 這是375屏幕 設計圖是750屏幕(2倍)
所以假設寬度86 在375屏幕就是43 同理fonsize 50在兩倍屏就是100
這樣計算rem就很簡單 直接用750屏去計算 86/100 = .86rem 
-->
<style lang="stylus" scoped>
@import '~styles/varibles.styl'

.header {
    display: flex
    line-height: .86rem
    background-color: $bgColor
    color: #fff
    .header-left {
        width: .64rem
        .back-icon {
            text-align: center
            font-size: .4rem
        }
    }
    .header-input {
        flex: 1
        height: .64rem
        line-height: .64rem
        margin-top: .12rem
        margin-left: .2rem
        background-color: #fff
        border-radius: .1rem
        color: #ccc
        padding-left: .2rem
    }
    .header-right {
        width: 1.24rem
        text-align center
        .arrow-icon {
            font-size: .24rem
        }
    }
}
</style>
