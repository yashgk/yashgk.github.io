function submitForm() {
    document.getElementById("contact_form").submit();
    document.getElementById("contact_form").reset();
    alert("Successfully Received! We will get back to you soon!");
    return false;
}


    <form action="https://formsubmit.co/2451e74427f4d6bece98030cf51a3ff0" method="POST" id="contact_form">
                        <!-- Honeypot -->
                        <input type="text" name="_honey" style="display: none;">

                        <!-- Disable captcha -->
                        <input type="hidden" name="_captcha" value="false">

                            <div class="input-control i-c-2">
                                <input type="text" required placeholder="YOUR NAME" name="name">
                                <input type="email" required placeholder="YOUR EMAIL" name="email">
                            </div>
                            <div class="input-control">
                                <input type="text" required placeholder="ENTER SUBJECT" name="subject">
                            </div>
                            <div class="input-control">
                                <textarea name="message" id="" cols="15" rows="8" placeholder="Message Here..."></textarea>
                            </div>
                            <!-- <input type="submit"> -->
                            <div class="submit-btn">   
                                <a href="#" id="submitbtn" class="main-btn" onclick="submitForm()">
                                    <span class="btn-text">Submit</span>
                                    <span class="btn-icon"><i class="fa-solid fa-paper-plane"></i></span>
                                </a>
                            </div>
                        </form>


                                .input-control {
            margin: 1.5rem 0;

            input,
            textarea {
                border-radius: 30px;
                font-weight: inherit;
                font-size: inherit;
                font-family: inherit;
                padding: .8rem 1.1rem;
                outline: none;
                border: none;
                background-color: var(--color-grey-5);
                width: 100%;
                color: var(--color-white);
                resize: none;
            }
        }

        .i-c-2 {
            display: flex;

            :last-child {
                margin-left: 1.5rem;
            }
        }

        .submit-btn {
            display: flex;
            justify-content: flex-start;
        }
