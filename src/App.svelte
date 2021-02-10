<script>
    import {MDBBtn, MDBJumbotron, MDBContainer, MDBRow, MDBCol, MDBIcon, MDBCard, MDBCardBody, MDBFooter} from "mdbsvelte";

    function toTop(){
        window.scrollTo({
            top: 0,
            left: 0,
            behavior: 'smooth'
        })
    }
</script>

<MDBJumbotron fluid>
    <MDBContainer>
        <div id="jumbo-padding">
        <MDBRow class="d-flex align-items-center">
            <MDBCol md="4" sm="12">
                <img class="img-fluid" src="https://cdn.statically.io/gh/wolfbyne/Simphiwe-Portfolio/main/public/images/circle-cropped-pp.png"  alt="Profile">
            </MDBCol>
            <MDBCol md="8" sm="12" class="text-center">
                <h2 class="display-4">Simphiwe Alpheus Nkosi</h2>
                <p class="lead">Sport Scientist - Sport Psychologist - Youth Football Coach</p>
            </MDBCol>
        </MDBRow>
        </div>
    </MDBContainer>
</MDBJumbotron>

<MDBContainer class="mt-5 mb-5 banner">
    <MDBRow class="d-flex align-items-center">
        <MDBCol md="6" sm="12">
            <a href="/Documents/Simphiwe-Resume.pdf" target='_blank'><MDBBtn size="lg" class="d-block mx-auto" gradient="aqua">Resume</MDBBtn></a>
        </MDBCol>
        <MDBCol md="6" sm="12">
            <img class="img-fluid" src="https://cdn.statically.io/gh/wolfbyne/Simphiwe-Portfolio/main/public/images/analysis-self.webp" alt="analysis">
        </MDBCol>
    </MDBRow>
  </MDBContainer>

<MDBContainer class="mt-5 mb-5 banner">
    <MDBRow class="d-flex align-items-center">
        <MDBCol md="6" sm="12">
            <img class="img-fluid" src="https://cdn.statically.io/gh/wolfbyne/Simphiwe-Portfolio/main/public/images/group-coach.webp" alt="coaches">
        </MDBCol>
        <MDBCol md="6" sm="12">
            <a href="/Documents/Simphiwe-Reference-Letter.pdf" target='_blank'><MDBBtn size="lg" class="d-block mx-auto" gradient="aqua">Reference Letter</MDBBtn></a>
        </MDBCol>
    </MDBRow>
</MDBContainer>

<MDBContainer class="mb-5 banner">
    <MDBCard>
        <MDBCardBody>
            <form>
                <p class="h4 text-center py-4">Contact Me</p>
                <label for="defaultFormCardNameEx" class="grey-text font-weight-light">
                    Your name
                </label>
                <input type="text" id="defaultFormCardNameEx" class="form-control"/>
                <br/>
                <label for="defaultFormCardEmailEx" class="grey-text font-weight-light">
                    Your email
                </label>
                <input type="email" id="defaultFormCardEmailEx" class="form-control"/>
                <br>
                <label for="subject" class="grey-text font-weight-light">Subject</label>
                <input type="text" id="subject" class="form-control" aria-describedby="emailHelp" placeholder="Enter your subject" name="subject">
                <br>
                <label for="Textarea" class="grey-text font-weight-light">Your message...</label>
                <textarea name="message" class="form-control" id="Textarea" rows="8"></textarea>
                <br>
                <MDBBtn class="d-block mx-auto" outline type="submit">
                    Send
                    <MDBIcon far icon="paper-plane" class="ml-2"/>
                </MDBBtn>
            </form>
        </MDBCardBody>
    </MDBCard>
</MDBContainer>

<MDBFooter color="default-color" class="font-small pt-4 mt-5">
    <MDBContainer fluid class="text-center text-md-left">
        <MDBRow>
            <MDBCol md="6" class="text-center">
                <h5 class="title">Simphiwe Alpheus Nkosi</h5>
                <p class="mt-2">Sport Scientist - Sport Psychologist - Youth Football Coach
                    <br> Houghton Estate, Johannesburg, South Africa
                </p>
                <div class="mt-1 mb-3">
                    <MDBIcon fas icon="map-marker-alt" size="2x"/>
                </div>
            </MDBCol>
            <MDBCol md="3">
                <h5 class="title mb-3">Socials</h5>
                <ul class="list-unstyled list-inline">
                    <li class="list-unstyled list-inline-item">
                        <a href="#!"><MDBIcon fab icon="facebook-square" size="3x"/></a>
                    </li>
                    <li class="list-unstyled list-inline-item">
                        <a href="mailto:nkosis@stjohnscollege.co.za"><MDBIcon fas icon="envelope-square" size="3x"/></a>
                    </li>
                    <li class="list-unstyled list-inline-item">
                        <a href="tel:+27768896093"><MDBIcon fas icon="phone-square" size="3x"/></a>
                    </li>
                </ul>
            </MDBCol>
            <MDBCol md="3">
                <MDBBtn class="mt-5" on:click={toTop} id="button">Scroll to top <MDBIcon fas icon="chevron-up" class="ml-3"/></MDBBtn>
            </MDBCol>
        </MDBRow>
    </MDBContainer>
    <div class="footer-copyright text-center py-3">
        <MDBContainer fluid>
            &copy; {new Date().getFullYear()} Copyright: <a href="https://splyce.dev"> SPLYCE </a>
        </MDBContainer>
    </div>
</MDBFooter>