<template lang="">
    <div>
        <h1>vs wordle</h1>

        <MainWordle />
        <WordleBoard />
        <!-- <RoundInfo></RoundInfo> -->
        <!-- <Previews></Previews> -->
        
    </div>
</template>

<script>
import MainWordle from './MainWordle.vue'
import WordleBoard from './WordleBoard.vue'

export default {
    name: 'GameDashboard',
    components: {
        MainWordle,
        WordleBoard

    },
    data: function () { return  { numberParticipants: 0, } }
}
</script>

<style>

h1 {
    color: #7C4B93;
    text-align: center;
    font: bold 72px Quicksand, sans-serif;
}

p.guest {
    color: #7C4B93;
    text-align: center;
    font: bold 32px Quicksand, sans-serif;
}

p.time {
    color: #7C4B93;
    text-align: center;
    font: bold 60px Quicksand, sans-serif;
}

body {
    background-color: #FCF2FF;
}

#mainrect {
    border-radius: 5px;
    background: #E7D0F1;
    padding: 10px;
    width: 456px;
    height: 773px;
}

#dashboard {
    border-radius: 5px;
    background: #E7D0F1;
    padding: 10px;
    width: 649px;
    height: 282px;
}

#textsquare {
    border-radius: 5px;
    background: #FCF2FF;
    padding: 10px;
    width: 456px;
    height: 773px;
}



</style>