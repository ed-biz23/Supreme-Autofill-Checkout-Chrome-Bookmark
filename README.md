# Supreme-Autofill-Checkout-Chrome-Bookmark

Simply copy the following code and save it as a bookmark on your chrome browser. Bookmark only works on deskptop. Also, supreme is known to change their html time to time so update may require.

<strong>How to use</strong>
- Once you add an item, click on the bookmark and it should take you to checkout page, and once the page is done loading, click on the bookmark for full checkout.

javascript: 
function checkOut(){
  document.getElementById('order_billing_name').value ='John Doe';
  document.getElementById('order_email').value ='johndoe@gmail.com';
  document.getElementById('order_tel').value ='0123456789';
  document.getElementById('bo').value ='123 Main st';
  document.getElementById('oba3').value ='1FL';
  document.getElementById('order_billing_zip').value ='12345';
  document.getElementById('order_billing_city').value ='Supreme';
  document.getElementById('order_billing_state').value ='NY';
  document.getElementById('nnaerb').value ='0000111122223333';
  document.getElementById('credit_card_month').value ='10';
  document.getElementById('credit_card_year').value ='2019';
  document.getElementById('orcer').value ='123';
  document.getElementsByClassName("has-checkbox terms")[0].click();
  document.getElementsByName("commit")[0].click()
}
if(location != 'https://www.supremenewyork.com/checkout') {
  location = 'https://www.supremenewyork.com/checkout';
} else {
  if(document.readyState === 'complete') {
    checkOut();
  }
} 
