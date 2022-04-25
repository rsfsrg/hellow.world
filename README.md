# hello.world

<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title> my website </title>
</head>
<style>
    :root {
        --gradient: linear-gradient(45deg,
                #ebfafa,
                #d6f5f5,
                #c2f0f0,
                #adebeb,
                #99e6e6,
                #85e0e0,
                #70dbdb,
                #4da6ff,
                #66b3ff,
                #80bfff,
                #99ccff,
                #b3d9ff,
                #cce6ff,
                #3399ff,
                #1a8cff,
                #0080ff,
                #0073e6,
                #0066cc,
                #0059b3,
                #004d99,
                #004080,
                #003366,
                #00264d);
        --gradient-2: linear-gradient(55deg,
                #3366ff,
                #1a53ff,
                #0040ff,
                #cc0099,
                #b30086,
                #990073);
    }

    body {

        font-family: tahoma;
        text-align: center;
        background-image: var(--gradient);
        background-size: 400%;
        animation: bg-animation 3s infinite alternate;
    }

    @keyframes bg-animation {
        0% {
            background-position: left;
        }

        100% {
            background-position: right;
        }
    }



    header {
        letter-spacing: 6px;
        background: royalblue;
        padding: 20px;
        color: white;
    }

    h2 {
        font-size: 2em;
        width: 100%;
    }

    section {
        padding: 30px;
        margin-bottom: 40px;
    }

    .container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
    }

    .card {
        border: 1px solid #ccc;
        background-color: ivory;
        margin: 25px;
        padding: 25px;
        box-shadow: rgba(110, 95, 95, 0.2);
    }

    .icon {
        font-size: 8em;
        padding: 25px;
    }

    button,
    .button {
        background: royalblue;
        border: 0;
        color: white;
        padding: 10px;
        width: 100%;
        margin-bottom: 100px;
    }

    @media screen and (min-width: 50em) {

        .card {
            flex-basis: 325px;
        }

        header h1 {
            font-size: 5em;
        }

    }

    .blue {
        background: teal;
    }

    td {
        padding: 10px;
    }

    table {
        margin: auto;
    }

    #my-order {
        background-color: #29c1c4;
        padding: 25PX;
        display: none;
    }

    .footer {
        background-color: gray;

    }
</style>

<body>
    <header>
        <h1>Noveler<h1>
                <h4>best novles of the world</h4>
    </header>
    <section>
        <h2>Welcome</h2>
        <p>vision is tell the world abut knowdlage of books which can bring everything to light</p> <br>
        <p>ABOUT US</p>
    </section>

    <section class=" blue container">
        <h2>service </h2>
        <article class="card">
            <div class="icon ">&#128509;
            </div>
            <h3>khan hunayya </h3>
            <p> a founder of this website she is a coder and also write novel her dream is to bring people knowlade that
                storys can teach peple nice think in different ways </p>
            <button>Contact</button>
        </article>
        <article class="card">
            <div class="icon "> &#128510;</div>
            <h3>khan zumar faris </h3>
            <p> the disturbe creater to this website also a writer of this website not mention every storys from zumar
                fairs is alsoways about lions well i will pass on that </p>
            <button>Contact</button>
        </article>

    </section>


    <section>
        <h2>
            my order forms
        </h2>
        <form id="my-form">
            <table>
                <tr>
                    <td> name: </td>
                    <td>
                        <input type="text" size="25" name="my-name">
                    </td>
                </tr>

                <tr>
                    <td> adress :</td>
                    <td><input type="text" size="25" name="my-name"></td>
                </tr>
                <tr>
                    <td> favorite book:</td>
                    <td>
                        <select name="my-book">
                            <option>Sherlock holmes</option>
                            <option>Halmet</option>
                            <option>secret seven adventure</option>
                            <option>Oliver twist</option>
                        </select>
                    </td>
                </tr>
                <tr>
                    <td>
                        Qunatity:
                    </td>
                    <td><input type="number" name="my-qty" value="1" min="1" max="10">
                        <small>(max 10)</small>
                    </td>
                </tr>
                <tr>
                    <br>
                    <div ID="my-order">

                    </div>
                </tr>
                <tr>
                    <td colspan="2">
                        <input type="button" value="process order " class="button" onclick="placeOrder();">
                        <input type="reset" value="clear" class="button"
                            onclick="document.getElementById('my-order').style.display ='none'" ;>
                    </td>
                </tr>

            </table>
        </form>
    </section>
    <di class="footer">
        <h3>thanks for visiting</h3>
        <div class="container">
            <article class="card">
                <h3>get in touch</h3>
                <p> best place to buys books where you will never find in normal store</p>
            </article>
            <article class="card">
                <h3>contact us</h3>
                <p>we should love to hear from you
                    <i>and you can even publish your books</i>
                    <br>email us or call us
                    mobile: 8324024753
                    email: youroushko@gmail.com
                    <br>

                    <strong> this is one of our publisher website you can wrtie storys and publish here </strong>
                    <i>publisher@gamil.com</i>
                </p>
            </article>
        </div>

    </di>

    <section class=" blue container">
        <h2>our team</h2>
        <article class="card">
            <div class="icon "> &#128512;</div>
            <h3>khan hanzala </h3>
            <p> one of our team member which help this website grow </p>
            <button>Contact</button>
        </article>
        <article class="card">
            <div class="icon "> &#128516;
            </div>
            <h3>khan ukkasha</h3>
            <p> he is also the best member of our team which takes out bug</p>
            <button>Contact</button>
        </article>



    </section>
    <h3>youroushko.com.in</h3>
    <script>


        function placeOrder() {
            var orderform = document.getElementById("my-form");
            results += "<br>name:" + orderform.element['my-name'].value;
            results += "<br>address:" + orderform.element['my-address'].value;
            results += "<br>i like do buy" + orderform.element['my-books'].value;
            results += "<bar>Qunatity:" + orderform.element['my-qty'].value;
            results = "<h3>Success!</h3> here is your order.";

            var orderResults = document.getElementById("my-order");
            orderResults.style.display = "block";
            orderResults.innerHTML = results;

        }
    </script>

</body>

</html>
