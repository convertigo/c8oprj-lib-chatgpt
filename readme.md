


# lib_ChatGPT

# This is the ChatGPT connector for Convertigo. 
This connector will enables Convertigo Applications to use the the ChatGPT AI engine for completions. Given a prompt, ChatGPT will answer and elaborate a response.



For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [Completion](#completion)
    - [forms_HandleBatchPrompts](#forms_handlebatchprompts)
    - [formssource_Prompt](#formssource_prompt)
- [Mobile Library](#mobile-library)


## Installation

1. In your Convertigo Studio use `File->Import->Convertigo->Convertigo Project` and hit the `Next` button
2. In the dialog `Project remote URL` field, paste the text below:
   <table>
     <tr><td>Usage</td><td>Click the copy button</td></tr>
     <tr><td>To contribute</td><td>

     ```
     lib_ChatGPT=https://github.com/convertigo/c8oprj-lib-chatgpt.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     lib_ChatGPT=https://github.com/convertigo/c8oprj-lib-chatgpt/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __lib_ChatGPT__ project


## Sequences

### Completion

The Completion API 

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>model</td><td>The model to be used can be : 
* text-davinci-003	
* text-curie-001
* text-babbage-001
* text-ada-001

</td>
</tr>
<tr>
<td>prompt</td><td>The prompt to ask to ChatGPT</td>
</tr>
<tr>
<td>temperature</td><td>Temperature , decimal from 0 to 1 ex: 0.6</td>
</tr>
</table>

### forms_HandleBatchPrompts

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>doc</td><td></td>
</tr>
<tr>
<td>originalDoc</td><td></td>
</tr>
</table>

### formssource_Prompt

Use this source in a Grid to display ChatGPT reponses to a prompt

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>forms_prompt</td><td>The prompt to ask to ChatGPT</td>
</tr>
</table>

## Mobile Library

Describes the mobile application global properties



