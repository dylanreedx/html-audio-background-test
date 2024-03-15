<script lang="ts">
    import svelteLogo from "./assets/svelte.svg";
    import viteLogo from "/vite.svg";
    import Counter from "./lib/Counter.svelte";
    import classOneDesign from "./assets/class-1-design.mp3";

    // get audio tag to play in background when a mobile device is off
    const audio = document.getElementById("class-audio") as HTMLAudioElement;
    if (audio) {
        audio.play();
    }
</script>

<main>
    <audio id="class-audio" controls>
        <source src={classOneDesign} type="audio/mpeg" />
    </audio>
</main>
