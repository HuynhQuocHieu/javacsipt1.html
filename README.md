<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <style>
            * {
                box-sizing: border-box;
                margin: 0;
                padding: 0;
            }
            section {
                display: flex;
                justify-content: center;
                height: 100%;
            }
            .container {
                display: flex;
                width: 60rem;
                height: 30rem;
                margin: auto;
                background: Violet;
            }
            .input-data {
                display: flex;
                justify-content: center;
                align-items: center;
                width: 100%;
                padding: 2em;
            }
            input[type="submit"],
            input[type="reset"] {
                width: 10rem;
                padding: .9em 0;
            }
            form > *,
            content > * {
                padding-bottom: 1em;
            }
            .flex {
                display: flex;
            }
            .gender > * {
                padding-left: 2em;
            }
            .hobby {
                flex-direction: column;
            }
            .hobby > * {
                padding-left: 2em;
                padding-bottom: .5em;
            }
            .button {
                padding: 0;
            }
            .output-data {
                display: flex;
                align-items: center;
                width: 100%;
                background: lightgreen;
            }
            .content > * {
                padding-left: 2em;
                padding-bottom: 1em;
            }
            @media (max-width: 60rem) {
                .container {
                    flex-direction: column;
                }
                .content {
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    height: 15rem;
                }
            }
        </style>
    </head>
    <body style="background:pink;">
        <section>
            <div class="container">
                <div class="input-data">
                    <form id="user-detail">

                        <div class="name">
                            <label for="name">T??n:</label>
                            <input type="text" id="user-name">
                        </div>
                        <div class="email">
                            <label for="name">Email:</label>
                            <input type="text" id="user-email">
                        </div>

                        <label for="gender">Gi???i T??nh:</label>
                        <div class="flex gender">
                            <div class="male">
                                <input type="radio" name="gender" value="Nam" id="user-gender">
<label for="male">Nam</label>
                            </div>
                            <div class="female">
                                <input type="radio" name="gender" value="N???" id="user-gender">
                                <label for="female">N???</label>
                            </div>
                        </div>

                        <div class="nation">
                            <label for="nation">Qu???c T???ch:</label>
                            <select name="nationality" id="user-nation">
                                <option>Vietnam</option>
                                <option>M???</option>
                                <option>Nh???t B???n</option>
                                <option>H??n Qu???c</option>
                                <option>Thailand</option>
                            </select>
                        </div>

                        <label for="hobby">S??? Th??ch:</label>
                        <div class="flex hobby">
                            <div class="coding">
                                <input type="checkbox" name="hobby" value="L???p Tr??nh">
                                <label for="coding">L???p Tr??nh</label>
                            </div>
                            <div class="Hotel">
                                <input type="checkbox" name="hobby" value=" ch??i game">
                                <label for="travel">ch??i game</label>
                            </div>
                        </div>

                        <div class="button">
                            <input type="submit" value="Ch???p Nh???n" id="submit">
                            <input type="reset" value="h???y" id="reset"/>
                        </div>
                    </form>
                </div>

                <div class="output-data">
                    <div class="content">
                        <p class="content-name">T??n:</p>
                        <p class="content-email">Email:</p>
                        <p class="content-gender">Gi???i T??nh:</p>
       
