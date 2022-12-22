<script>
    let noteIndex = 1;
    let noteTitle = "The problems with analogies and the possible ways to fix them.";
    let noteContent = "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim totam nisi, modi et aliquid error aut unde non quia, nostrum pariatur rerum voluptatum aperiam obcaecati. Accusantium odit ducimus placeat possimus!";
    let noteAuthor = "Adwait";

</script>


<div class="nav">
    <h2>Observing </h2> 
    <input type="text" placeholder={noteIndex.toString()}>
</div>
<div class="page">
    <div class="header">
        <h1>{noteTitle}</h1>
        <div class="fold"></div>
    </div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

    .nav {
        position: relative;
        align-self: flex-start;
        display: flex;
        gap: 0.5em;
        margin-bottom: 20px;
    }

    .nav h2  {
        width: min-content;
        display: inline-block;
        font-family: 'Montserrat';
        font-weight: 300;
        font-style: italic;
        font-size: 3.1em;
    }

    .nav input, .nav input:active, .nav input:focus {
        background: transparent;
        border: none;
        outline: #232323 solid 1px;

        flex: 1;
        width: 100%;

        font-size: 4.2em;
        font-family: 'Montserrat';
        font-style: italic;
        font-weight: 700;
    }

    .nav input::placeholder {
        color: rgb(55, 55, 55);
    }

    .header h1 {
        padding-left: 0em;
        padding-top: 0.5em;
        font-family: 'Montserrat';
        font-weight: 800;
        font-size: 2.6rem;
        width: fit-content;
    }

    @media only screen and (min-width: 925px){

        .header h1 {
            padding-left: 0.8em;
            padding-right: 0.5em;
            padding-top: 0.5em;
            font-family: 'Montserrat';
            font-weight: 800;
            font-size: 3rem;
        }

        .page {
            position: relative;
            border: 1px solid whitesmoke;
            width: 70vw;
            height: 200vh;
        }

        .header {
            height: fit-content;
            display: flex;
            justify-content: space-between;
            align-content: flex-start;

        }

        .fold {
            position: relative;
            left: 2px;
            top: -2px;
            background-color: #151515;
            border-left: 135px solid white;
            border-top: 135px solid #151515;
            width: 0%;
            height: 0%;
        }
    }
    

</style>