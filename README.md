# paypalextended
Paypal Extended for osclass
This plugin lets you to add more than 3 packages for paypal payments.

To add more packages files needed to changes are the below:
index.php
Line number
36-41
example to add extra package name
osc_set_preference('pack_price_7', '', 'paypal', 'STRING');

Line number 
83-88
osc_delete_preference('pack_price_7', 'paypal');


====
user_menu_pack.php
Line number 1-20
if(osc_get_preference("pack_price_7", "paypal")!='' && osc_get_preference("pack_price_7", "paypal")!='0') {
        $packs[] = osc_get_preference("pack_price_7", "paypal");
    }

Line number 40-63
add the names to your package
    




