CkHelper
========

CK Helper for CakePHP

Steps to Install

1) Download CkEditor and place it in the folder
app/webroot/js/ckeditor

2) In your controller, or in AppController.php add the following like of code:

public $helpers = array('Ck')

3) In your layout file (default is in app/View/Layouts/default.ctp) add the following line in your <head> section:

echo $this->Html->script('ckeditor/ckeditor.js');

4) Now in your view file, when you want to call the CK editor, you can use:

echo $this->Ck->input('field_name');

Or

echo $this->Ck->input('Model.field_name');

Other options include:

echo $this->Ck->input('Model.field_name', array('label' => 'Custom Label'));

Hopefully this comes in use for some of you!
