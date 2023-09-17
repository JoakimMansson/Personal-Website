<div class="ProjectsBar">
    <div class="grid-item">
        <h1>Projects</h1>
    </div>
    <div class="grid-item">
        <p>Hej här</p>
    </div>
</div>

<style>
    .ProjectsBar {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: auto;
        position: absolute;
        top: 1300px;
        text-align: center;
        color: white;
        font-family: 'Roboto Mono', monospace;
        gap: 10px;
    }

    .grid-item {
        background-color: #f2f2f2;
        padding: 20px;
        text-align: center;
    }

    /* Define specific positions for grid items */
    .grid-item:nth-child(1) {
      grid-column: 1 / 3; /* Item 1 spans from column 1 to column 3 */
      grid-row: 1; /* Item 1 is in row 1 */
    }

</style>