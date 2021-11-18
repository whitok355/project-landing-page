<template>
    <div class="b-container">
        <div class="b-boxes-help">
            <div class="b-boxes-help__box">
                <div class="b-boxes-help__titleBox">
                    <div class="b-boxes-help__border"></div>
                    <div class="b-boxes-help__title b-relative">Weight Lifting</div>
                </div>
            </div>
            <div class="b-boxes-help__box">
                <div class="b-boxes-help__titleBox">
                    <div class="b-boxes-help__border"></div>
                    <div class="b-boxes-help__title b-relative">Running & Spinning</div>
                </div>
            </div>
            <div class="b-boxes-help__box">
                <div class="b-boxes-help__titleBox">
                    <div class="b-boxes-help__border"></div>
                    <div class="b-boxes-help__title b-relative">Pumping Iron</div>
                </div>
            </div>
            <div class="b-boxes-help__box">
                <div class="b-boxes-help__titleBox">
                    <div class="b-boxes-help__border"></div>
                    <div class="b-boxes-help__title b-relative">Pumping Iron</div>
                </div>
            </div>
        </div>
        <div class="b-boxes-help">
            <div class="b-list-box">
                <div class="b-list-box__container">
                    <div class="b-list-box__border"></div>
                    <div class="b-list-box__title b-relative">Physical Health</div>
                </div>
            </div>
            <div class="b-list-box">
                <div class="b-list-box__container">
                    <div class="b-list-box__border"></div>
                    <div class="b-list-box__title b-relative">Mental Health</div>
                </div>
            </div>
            <div class="b-list-box">
                <div class="b-list-box__container">
                    <div class="b-list-box__border"></div>
                    <div class="b-list-box__title b-relative">Nutrition</div>
                </div>
            </div>
            <div class="b-list-box">
                <div class="b-list-box__container">
                    <div class="b-list-box__border"></div>
                    <div class="b-list-box__title b-relative">Gymnastics</div>
                </div>
            </div>
            <div class="b-list-box">
                <div class="b-list-box__container">
                    <div class="b-list-box__border"></div>
                    <div class="b-list-box__title b-relative">Crossfit</div>
                </div>
            </div>
            <div class="b-list-box">
                <div class="b-list-box__container">
                    <div class="b-list-box__border"></div>
                    <div class="b-list-box__title b-relative">Aerobics</div>
                </div>
            </div>
        </div>
        <div class="b-boxes-help">
            <div class="b-discr-box">
                <div class="b-discr-box__content">
                    <div class="b-discr-box__title">Nutritional Plans</div>
                    <div
                        class="b-discr-box__text"
                    >Nutritional Facts on some shitty things that you don’t care about and even we don’t , I need to replace this copy.</div>
                </div>
            </div>
            <div class="b-discr-box">
                <div class="b-discr-box__content">
                    <div class="b-discr-box__title">Weight Loss</div>
                    <div
                        class="b-discr-box__text"
                    >Nutritional Facts on some shitty things that you don’t care about and even we don’t , I need to replace this copy.</div>
                </div>
            </div>
            <div class="b-discr-box">
                <div class="b-discr-box__content">
                    <div class="b-discr-box__title">Mental Peace</div>
                    <div
                        class="b-discr-box__text"
                    >Nutritional Facts on some shitty things that you don’t care about and even we don’t , I need to replace this copy.</div>
                </div>
            </div>
            <div class="b-discr-box">
                <div class="b-discr-box__content">
                    <div class="b-discr-box__title">Home Training</div>
                    <div
                        class="b-discr-box__text"
                    >Nutritional Facts on some shitty things that you don’t care about and even we don’t , I need to replace this copy.</div>
                </div>
            </div>
            <div class="b-discr-box">
                <div class="b-discr-box__content">
                    <div class="b-discr-box__title">Work/Life Balance</div>
                    <div
                        class="b-discr-box__text"
                    >Nutritional Facts on some shitty things that you don’t care about and even we don’t , I need to replace this copy.</div>
                </div>
            </div>
            <div class="b-discr-box">
                <div class="b-discr-box__content">
                    <div class="b-discr-box__title">Cardio</div>
                    <div
                        class="b-discr-box__text"
                    >Nutritional Facts on some shitty things that you don’t care about and even we don’t , I need to replace this copy.</div>
                </div>
            </div>
        </div>
    </div>
</template>
<script></script>
<style lang="scss">
.b-boxes-help {
    display: flex;
    justify-content: space-evenly;
    flex-direction: column;
    align-items: center;
    margin-top: 24px;

    &__box {
        width: 350px;
        height: 350px;
        display: flex;
        font-size: 32px;
        line-height: 34px;
        color: #ffffff;
    }
    &__titleBox {
        letter-spacing: -0.006em;
        padding: 78px 52px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    &__border {
        width: 249px;
        border-top: 2px solid white;
    }
    &__title {
        padding-top: 24px;
        max-width: 220px;
    }
    &__title::before {
        content: "";
        display: inline-block;
        padding: 5px;
        border-radius: 100px;
        background: #e9b730;
        position: absolute;
        top: 34px;
        left: -23px;
    }
    &__box {
        margin-bottom: 10px;
    }
    &__box:nth-child(1) {
        background: #ffe2de;
    }
    &__box:nth-child(2) {
        background: #c4e769;
    }
    &__box:nth-child(3) {
        background: #62d0df;
    }
    &__box:nth-child(4) {
        background: #0052c1;
    }

    @media (min-width: 768px) {
        & {
            flex-direction: row;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        &__box {
            margin-right: 3px;
            margin-bottom: 5px;
        }
    }
}
.b-list-box {
    width: 350px;
    height: 350px;
    display: flex;
    justify-content: center;
    margin-bottom: 10px;

    &:nth-child(1) {
        background: #22356f;
    }
    &:nth-child(2) {
        background: #0052c1;
    }
    &:nth-child(3) {
        background-image: url("../assets/images/strawberry.png");
        background-position: center center;
        background-size: cover;
        background-repeat: no-repeat;
    }
    &:nth-child(4) {
        background: #62d0df;
    }
    &:nth-child(5) {
        background: #dee1ff;
    }
    &:nth-child(6) {
        background: #8f00ff;
    }
    &__container {
        padding-top: 96px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    &__border {
        border-top: 2px solid #ffffff;
        width: 249px;
    }
    &__title {
        padding-top: 24px;
        font-size: 32px;
        line-height: 34px;
        letter-spacing: -0.006em;
        color: #ffffff;
    }
    &__title::before {
        content: "";
        display: inline-block;
        padding: 5px;
        border-radius: 100px;
        background: #e9b730;
        position: absolute;
        top: 34px;
        left: -23px;
    }
    @media (min-width: 768px) {
        & {
            margin-right: 3px;
            margin-bottom: 5px;
        }
    }
    @media (min-width: 1440px) {
        & {
            width: 460px;
            height: 460px;
        }
    }
}
.b-discr-box {
    width: 350px;
    height: 240px;

    &__content {
        display: flex;
        justify-content: center;
        flex-direction: column;
        padding: 55px 48px;
    }
    &__title {
        font-size: 28px;
        line-height: 33px;
        letter-spacing: -0.03em;
        color: #22356f;
    }
    &__text {
        padding-top: 28px;
        font-size: 16px;
        line-height: 25px;
        letter-spacing: -0.03em;
        color: rgba(34, 53, 111, 0.5);
    }
    @media (min-width: 1440px) {
        & {
            width: 480px;
            height: 240px;
        }
        &__content {
            padding: 55px 77px 55px 105px;
        }
    }
}
</style>