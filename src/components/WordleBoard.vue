<template lang="">
<!-- // represents a wordle board
// has the option of hiding the letters
// does not include the keyboard
-->
    <div> 
        <h1>
            HELLO
        </h1>
        <div id="board">
            <div
                v-for="row in board"
                :class="row"
                :key="row"
            >
                <div
                    v-for="tile in row"
                    :class="['tile']"
                    :key="tile"
                >
                    {{ tile.letter }}
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data: function () {
        return {
            guessesSoFar: [],
            boardStates: Array.from({ length: 6 }, () => 
                Array.from({ length: 5 }, () => (
                    {
                        // TODO: the A heree is a substitute letter
                        letter: 'A',
                        state: false
                    }
                ))),
            showLetters: true
            }
    }
    
}
</script>

<style>
.board {
    background-color: #fff;
    width: 400px;
} 
</style>