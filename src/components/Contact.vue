<template>
    <div id="contact" class="paddsection">
    <div class="container">
      <div class="contact-block1">
        <div class="row">
          <div class="col-lg-6">
            <div class="contact-contact">
              <h2 class="mb-30">Restons Connectés</h2>
              <ul class="contact-details">
                <li><span>Karma Music</span></li>
                <li><span>Christophe A (Manager)</span></li>
                <li><span>"Dad"</span></li>
                <li><span>0690494428 / 0690275708</span></li>
                <li><span>karmamusicstaff@gmail.com</span></li>
              </ul>
            </div>
          </div>
          <div class="col-lg-6">
            <form action="" method="post" role="form" class="contactForm">
              <div class="row">
                <div id="sendmessage">Votre message a bien été envoyé</div>
                <div id="errormessage"></div>
                <div class="col-lg-6">
                  <div class="form-group contact-block1">
                    <input type="text" name="name" class="form-control" id="name" placeholder="Votre nom" data-rule="minlen:4" data-msg="Entrez votre nom" />
                    <div class="validation"></div>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="form-group">
                    <input type="email" class="form-control" name="email" id="email" placeholder="Votre adresse email" data-rule="email" data-msg="Entrez une adresse mail valide" />
                    <div class="validation"></div>
                  </div>
                </div>
                <div class="col-lg-12">
                  <div class="form-group">
                    <input type="text" class="form-control" name="subject" id="subject" placeholder="Sujet" data-rule="minlen:4" data-msg="Entrez le sujet de votre message" />
                    <div class="validation"></div>
                  </div>
                </div>
                <div class="col-lg-12">
                  <div class="form-group">
                    <textarea class="form-control" name="message" rows="12" data-rule="required" data-msg="Entrez votre message" placeholder="Votre message"></textarea>
                    <div class="validation"></div>
                  </div>
                </div>
                <div class="col-lg-12">
                  <input type="submit" class="btn btn-defeault btn-send" value="Envoyer">
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name:'Contact'
}
</script>

<style>

</style>
