+++
title = 'Create Language-specific Workflow Messages for a Category'
solution = 'Master Data Management'
+++

# Create Language-specific Workflow Messages for a Category

dspConduct™ sends Workflow messages to users as a request moves through
the workflow. By default, these messages are in English.

If the notification text must use a language other than English, a
Designer should create Category Workflow Language Messages for each
relevant language that is marked Active in DSP®, though this is not
required..  

<span style="font-weight: bold;">NOTE</span>: Regardless of the
notification's language, a Designer must navigate to the [Category
Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm) page for
workflow messages to be created.  If a Designer does not navigate to the
page, workflow messages are not sent.

To navigate to the page:

1.  Click <span style="font-weight: bold;">dspConduct\> Design</span> in
    the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.

3.  Click the <span style="font-weight: bold;">Workflow Messages</span>
    icon.

4.  Click the <span style="font-weight: bold;">Messages</span> icon for
    a language.

Category Workflow Language Messages are initially created with the
values from the Workflow Message Defaults. Refer to [View Default
Workflow Messages](View_Default_Workflow_Messages.htm) for more
information.

The message body text may be changed to the language-specific text.  The
default Email From value should be changed to a valid email address that
pertains to a client’s site, though this is not required. The email
messages use this client-supplied address in the Email From field in the
messages.  

To change the message body text and set the Email From:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.

3.  Click the <span style="font-weight: bold;">Workflow Messages</span>
    icon.

4.  Click the <span style="font-weight: bold;">Messages</span> icon for
    a language.

5.  Click <span style="font-weight: bold;">Edit</span> for a message.
    
    [View the field descriptions for the Category Workflow Language
    Message page](../Page_Desc/Category_Workflow_Language_Message_H.htm)

6.  Change the message body text to the language-specific text if
    applicable in the <span style="font-weight: bold;">MESSAGE</span>
    field.
    
    **NOTE**: Do not replace the values enclosed with \#.:
    
    **NOTE**: The default (email@ClientDomain.com) should be replaced
    with a valid client-supplied email address, though this is not
    required.  

7.  Enter the email address in the<span style="font-weight: bold;">
    EMAIL FROM</span> field.

8.  Click <span style="font-weight: bold;">Save</span>.
