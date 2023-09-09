<script>

</script>

<div class="Expertise">
    <div class="container">
        <div class="box">
            <div class="box-icon">
                <img src="icon1.png" alt="Icon 1">
            </div>
            <div class="box-text">
                <h2>Box 1</h2>
                <p>This is the text for Box 1.</p>
            </div>
        </div>
    
        <div class="box">
            <div class="box-icon">
                <img src="icon2.png" alt="Icon 2">
            </div>
            <div class="box-text">
                <h2>Box 2</h2>
                <p>This is the text for Box 2.</p>
            </div>
        </div>
    
        <div class="box">
            <div class="box-icon">
                <img src="icon3.png" alt="Icon 3">
            </div>
            <div class="box-text">
                <h2>Box 3</h2>
                <p>This is the text for Box 3.</p>
            </div>
        </div>
    </div>
</div>

<style>
    .Expertise {
        position: absolute;
        top: 2000px;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
        color: white;
        font-family: 'Roboto Mono', monospace;
    }

    .container {
    display: flex;
    flex-wrap: wrap; /* Wrap items to the next line if there isn't enough space */
    justify-content: space-between; /* Distribute items evenly with space in between */
    }

    .box {
        border: 2px solid #fff; /* White border */
        padding: 20px; /* Add spacing inside the box */
        width: calc(33.33% - 20px); /* Set the desired width for the boxes (33.33% to fit 3 boxes per row) */
        margin-bottom: 20px; /* Add margin between boxes (both horizontal and vertical) */
    }

    .box-icon {
        text-align: center; /* Center the icon */
    }

    .box-icon img {
        width: 50px; /* Set the width of the icon */
        height: 50px; /* Set the height of the icon */
        display: block; /* Remove any extra spacing */
        margin: 0 auto; /* Center the icon horizontally */
    }

    .box-text h2 {
        font-size: 18px; /* Adjust the heading font size */
        margin-top: 10px; /* Add spacing above the heading */
    }

    .box-text p {
        font-size: 14px; /* Adjust the paragraph font size */
        margin-top: 10px; /* Add spacing above the paragraph */
    }
</style>