<script>
    import VideoPlayer from "$lib/VideoPlayer.svelte";
</script>

<svelte:head>
	<title>Fantasy 101 | League Of Record</title>
</svelte:head>

<main>
    <div class="content-container">
        <h2>Fantasy Football 101</h2>

        <div class="top-content-row">
            <div class="image-wrapper">
                <img src="/fantasy-terms.png" alt="Fantasy Football Terms" />
            </div>
            <div class="image-wrapper">
                <img src="/scoring-format.png" alt="Scoring Format" />
            </div>
            <div class="image-wrapper">
                <img src="/draft-board.png" alt="Fantasy Football Draft Board" />
            </div>
            <div class="image-wrapper">
                <img src="/fantasy101.png" alt="Fantasy Football Draft Strategies" />
            </div>
        </div>

        <h2>Position Tiers</h2>
        <div class="tier-images-row">
            <div class="image-wrapper">
                <img src="/QBTiers.png" alt="Quarterback Tiers" />
            </div>
            <div class="image-wrapper">
                <img src="/RBTiers.png" alt="Running Back Tiers" />
            </div>
            <div class="image-wrapper">
                <img src="/WRTiers.png" alt="Wide Receiver Tiers" />
            </div>
            <div class="image-wrapper">
                <img src="/TETiers.png" alt="Tight End Tiers" />
            </div>
        </div>
        
        <h2>Important Videos</h2>
        <div class="video-container-row">
            <div class="video-wrapper">
                <p>How to play (Please watch if new!)</p>
                <VideoPlayer videoId="UApjbalTgTw" />
            </div>
            <div class="video-wrapper">
                <p>FAAB Waiver explained (Please Watch!!)</p>
                <VideoPlayer videoId="9DbceKcVl24" />
            </div>
            <div class="video-wrapper">
                <p>Hero RB explained</p>
                <VideoPlayer videoId="gjMc0teBulU" />
            </div>
            <div class="video-wrapper">
                <p>5 Draft tips</p>
                <VideoPlayer videoId="9AuYKY_vHdI" />
            </div>
            <div class="video-wrapper">
                <p>Finding late round RBs</p>
                <VideoPlayer videoId="sxAKw2g25MQ" />
            </div>
            <div class="video-wrapper">
                <p>QB draft strategy</p>
                <VideoPlayer videoId="jMBaRlGCat8" />
            </div>
            <div class="video-wrapper">
                <p>Draft Strats</p>
                <VideoPlayer videoId="g2ujCbT5TYY" />
            </div>
        </div>
    </div>
</main>

<style>
    .content-container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 2em;
        text-align: left;
    }
    
    .top-content-row, .tier-images-row {
        display: flex;
        justify-content: space-around;
        gap: 2em;
        margin-bottom: 2em;
        flex-wrap: wrap;
    }

    .image-wrapper {
        flex: 1;
        text-align: center;
        min-width: 200px;
    }
    
    .image-wrapper img {
        width: 100%;
        max-width: 450px;
        height: auto;
        display: block;
        margin: 0 auto;
    }

    h1, h2 {
        text-align: center;
        margin-top: 0.5em;
    }

    .video-container-row {
        display: flex;
        justify-content: flex-start;
        gap: 2em;
        margin-bottom: 2em;
        flex-wrap: wrap;
    }

    .video-wrapper {
        flex: 1;
        min-width: 300px;
    }

    /* Responsive styles for smaller screens */
    @media (max-width: 768px) {
        .top-content-row, .tier-images-row {
            flex-direction: column;
        }
        .image-wrapper {
            margin-bottom: 1em;
            min-width: unset;
        }
        .video-container-row {
            justify-content: center;
        }
        .video-wrapper {
            width: 100%;
        }
    }
</style>
