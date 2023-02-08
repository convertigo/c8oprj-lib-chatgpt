


# lib_ChatGPT

# This is the ChatGPT connector for Convertigo. 
This connector will enables Convertigo Applications to use the the ChatGPT AI engine for completions. Given a prompt, ChatGPT will answer and elaborate a response.



For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [Completion](#completion)
    - [forms_HandleBatchPrompts](#forms_handlebatchprompts)
    - [formssource_Prompt](#formssource_prompt)
    - [HandleBatchPrompts](#handlebatchprompts)
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
text-davinci-003, 
text-curie-001, 
text-babbage-001, 
text-ada-001


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

This No Code action will handle ChatGPT prompts in batch mode.

The action will use a CSV file uploaded in a No Code Studio (Forms) app and will execute all lines of this CSV file against the API.

The file format must have these columns

|title|definition_gpt|prompt_prefix|Prompt_suffix|prompt|model|max_tokens|temperature|top_p|frequency_penalty|presence_penalty|
|-----|--------------|-------------|-------------|------|-----|----------|-----------|-----|-----------------|----------------|
|optional|Optional   |A prefix to the prompt | the prompt itself | a suffix to the prompt | the model to be used | max number for tokens (words) | temperatuer (randomicity..) | optional |  optional | optional | 



**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>doc</td><td>The No Code app response doc</td>
</tr>
<tr>
<td>forms_email</td><td>The email where ChatGPT responses must be emailed to</td>
</tr>
<tr>
<td>originalDoc</td><td>The No Code app form</td>
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

### HandleBatchPrompts

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>batchFile</td><td></td>
</tr>
<tr>
<td>toEmail</td><td></td>
</tr>
</table>

## Mobile Library

Describes the mobile application global properties



