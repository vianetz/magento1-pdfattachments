Vianetz PDF Attachments Extension
=====================

Facts
-----
- version: 1.0.1

Description
-----------
This extension provides methods to attach documents to Magento emails, i.e. it does not have any configuration or
does anything out of the box. You can use it to base your own Magento extensions on it.

Additionally the extensions introduces the following new events to hook into the email sending process:
- vianetz_pdfattachments_email_template_init
- vianetz_pdfattachments_email_send_before
- vianetz_pdfattachments_email_send_after

You can use the following helper method to attach any document to an email, e.g. in the _email\_send\_before_ event:
```php
Mage::helper('vianetz/pdfattachments')->addAttachmentToEmail(Mage_Core_Model_Email_Template $emailTemplate, $fileContents, $filename);
```

A sample implementation of the usage of this module can be found in our [Advanced Invoice Layout Extension for Magento](https://www.vianetz.com/advancedinvoicelayout).

Requirements
------------
- PHP >= 5.3.6
- Magento >= 1.6.x

Frequently Asked Questions
--------------------------
Please find the Frequently Asked Questions on our website www.vianetz.com/en/faq.

Support
-------
If you have any issues or suggestions with this extension, please do not hesitate to
contact me at https://www.vianetz.com/en/contacts or support@vianetz.com.

Developer
---------
Christoph Massmann
[http://www.vianetz.com](http://www.vianetz.com)
[@vianetz](https://twitter.com/vianetz)

Licence
-------
[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)

See also LICENSE file.

Copyright
---------
(c) since 2008 vianetz

This Library uses Semantic Versioning - please find more information at http://semver.org.
