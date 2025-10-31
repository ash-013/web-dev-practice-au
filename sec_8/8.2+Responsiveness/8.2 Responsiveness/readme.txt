Main ways of responsive design:

1: Media Queries

    @media (max-width: 600px){
        /* CSS code */
    }


2: CSS Grid

    Great for creating a 2-D layout

    <div class="grid-container">
        <div class="first card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
        <div class="card"></div>
    </div>

    .grid-container{
        display: grid;
        grid-template-rows: 100px 200px 200px;
        grid-template-columns: 1fr 1fr;
        gap: 30px
    }

    .first{
        grid-column: span 2;
    }

    .card{
        background-color: blue;
    }



3: CSS Flexbox

    Allowing us to create 1-D layout

    <div class="flex-container">
        <div class="first card"></div>
        <div class="second card"></div>
        <div class="card"></div>
        <div class="card"></div>
    </div>

    .flexbox-container{
        display: flex;
    }

    .card{
        background: blue;
        border: 30px solid white;
        height: 100px
        flex: 1
    }

    .first{
        flex: 2;
    }

    .second{
        flex: 0.5;
    }



4: External FrameWorks (example: BootStrap)

    <div class="container">
        <div class="row">
            <div class="card col-6">
                Card
            </div>
            <div class="card col-2">
                Card
            </div>
            <div class="card col-4">
                Card
            </div>
        </div>
    </div>