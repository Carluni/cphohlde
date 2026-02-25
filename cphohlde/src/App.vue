<script setup lang="ts">
import BaseTile from './components/BaseTile.vue';
import HeadingTile from './components/HeadingTile.vue';
import ImageTile from './components/ImageTile.vue';
import TextTile from './components/TextTile.vue';
import panda from './assets/_Q0A4405.jpg'
import winter from './assets/_Q0A4405-5.jpg'
import stump from './assets/_Q0A4405-6.jpg'
import flowers from './assets/_Q0A4405-7.jpg'
import marshes from './assets/_Q0A4405-1.jpg'
import eiffel from './assets/_Q0A4405-2.jpg'
import hooks from './assets/_Q0A4405-8.jpg'
</script>

<template>
    <div class="fixed inset-0 -z-10 w-full h-full bg-black">
        <img src="./assets/_Q0A4405-9.jpg" class="h-full w-full object-cover grayscale opacity-20">
    </div>
    <div class="flex h-base">
        <BaseTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>

        <BaseTile>
        </BaseTile>
        <BaseTile class="w-quad">
            <HeadingTile>Hi, I'm Carl.</HeadingTile>
        </BaseTile>



        <BaseTile>
        </BaseTile>


    </div>
    <div class="flex h-base">
        <BaseTile class="w-base">

        </BaseTile>
        <BaseTile class="w-double">
            <ImageTile :src="flowers">
                Shot on film, developed manually.
            </ImageTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>
        <BaseTile class="h-double">
            <TextTile>I take photos on film and sometimes digitally. Also, I do my PhD in Electrical Engineering.
            </TextTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>
        <BaseTile>
            <ImageTile :src="stump">
                It's a tree but I think it's beautiful.
            </ImageTile>
        </BaseTile>

        <BaseTile>
        </BaseTile>
        <BaseTile>
            <ImageTile :src="panda">
                This panda walks our local zoo. It just mated.
            </ImageTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>
    </div>
    <div class="flex h-base">
        <BaseTile>
        </BaseTile>
        <BaseTile class="w-base">
            <HeadingTile>Try shooting film!</HeadingTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>

        <BaseTile class="h-double">
            <ImageTile :src="eiffel">
                I know it's cliché. Don't judge.
            </ImageTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>
        <BaseTile class="h-double">
            <ImageTile :src="winter">
                Shot on film
            </ImageTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>
        <BaseTile>
            <ImageTile :src="hooks">
                I'm sorry, pigs.
            </ImageTile>
        </BaseTile>
    </div>
    <div class="flex h-base">
        <BaseTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>
        <BaseTile class="w-base">
            <TextTile>I sometimes try web development. But judge for yourself if I am good at it.</TextTile>
        </BaseTile>
        <BaseTile>
                    </BaseTile>
        <BaseTile>
                    </BaseTile>
        <BaseTile>
                    </BaseTile>
        <BaseTile class="w-base">
            <TextTile>I develop pictures at home and scan</TextTile>
        </BaseTile>

        <BaseTile class="w-double">
            <ImageTile :src="marshes">
                This is how salt is made in southern france.
            </ImageTile>
        </BaseTile>
        <BaseTile>
        </BaseTile>

    </div>

</template>

<style scoped></style>
