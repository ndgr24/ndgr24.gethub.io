<form method="post" action="//submit.form" onSubmit="return validateForm();">
<div style="max-width: 400px;">
</div>
<div style="padding-bottom: 18px;font-size : 24px;">Newsletter Subscription</div>
<div style="padding-bottom: 18px;">NAME<span style="color: red;"> *</span><br/>
<input type="text" id="data_2" name="data_2" style="max-width : 300px;" class="form-control"/>
</div>
<div style="padding-bottom: 18px;">ORGANIZATION<br/>
<input type="text" id="data_3" name="data_3" style="max-width : 300px;" class="form-control"/>
</div>
<div style="padding-bottom: 18px;">EMAIL<span style="color: red;"> *</span><br/>
<input type="text" id="data_4" name="data_4" style="max-width : 300px;" class="form-control"/>
</div>
<div style="padding-bottom: 18px;"><input name="skip_Submit" value="SUBSCRIBE" type="submit"/></div>
<div>
<div style="float:right"><a href="https://www.100forms.com" id="lnk100" title="form to email">form to email</a></div>
<script src="https://www.100forms.com/js/FORMKEY:GBHELDXNUJX8/SEND:my@email.com" type="text/javascript"></script>
</div>
</form>

<script type="text/javascript">
function validateForm() {
if (isEmpty(document.getElementById('data_2').value.trim())) {
alert('NAME is required!');
return false;
}
if (isEmpty(document.getElementById('data_4').value.trim())) {
alert('EMAIL is required!');
return false;
}
if (!validateEmail(document.getElementById('data_4').value.trim())) {
alert('EMAIL must be a valid email address!');
return false;
}
return true;
}
function isEmpty(str) { return (str.length === 0 || !str.trim()); }
function validateEmail(email) {
var re = /^([\w-]+(?:\.[\w-]+)*)@((?:[\w-]+\.)*\w[\w-]{0,66})\.([a-z]{2,15}(?:\.[a-z]{2})?)$/i;
return isEmpty(email) || re.test(email);
}
</script>
