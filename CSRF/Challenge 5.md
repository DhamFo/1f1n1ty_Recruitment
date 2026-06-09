CSRF where token is tied to non-session cookie:
    -In this the application does not check if the CSRF token is matching with users token insted it compare with csrkey
    -As long as both the CSRF token and csrfkey are same no problem occurs.
    -Because of that an attacker can overwrite a victim's csrfKey cookie
    -"Solution will be updated soon after finding a way :) "