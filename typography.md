---
layout: page
title: Project
permalink: /project/
main_nav: true
---

<h1 id = "headings"> PAFMIM </h1>
<p style="text-align: justify;">
Foundation models are huge models in the terms of number of parameters, neurons, layers, etc. which are pre trained on huge amounts of data. These can be later adapted for various downstream tasks using small amounts of data and reduced computation through fine-tuning, transfer learning, or prompt engineering. Due to recent advancements, powerful foundational models exist which can be used for visual tasks to be performed well by being used as feature extractors, and then used for other downstream tasks by adaptation.
In this project we aim to leverage these foundation models and advanced learning paradigms to address the complexities of the highly sensitive medical domain, with a particular focus on CT and MRI data.
<br>
This endeavor presents us with two key challenges. First, bridging the domain gap between the training data of foundation models which are natural images and that of the application domain which consists of medical images. The gap leads to differences in the semantics, granularity and dimensionality of the images. Thus for the adaptation of the foundation models we need novel data processing and learning methods. Second, due to the sensitive nature  of medical data and strict privacy laws around it, we need to ensure strong privacy guarantees to prevent leakage of private data. Both input and output adaptations need to be made using novel methods to stop data leakage from either the model or its predictions.
<br>
While the primary goal is to adapt foundational models for the analysis of CT and MRI data, this project is poised to have a broader impact. The associated research will lead to adaptation of foundational models to the medical domain while maintaining performance and developing advanced learning paradigms that provide privacy guarantees while using the strong feature extractor capacities of foundational models. We will make all our developed methods available as open-source code, allowing them to be adopted for practical use. The novel methods learnt as a result would also be useful in other domains with similar challenges. For instance, in automated driving there also exists a similar gap in the domain of training data and in the case of applications like face recognition and biometrics, they face the challenge of usage of highly sensitive data. Thus our methods have the potential to tackle such tasks.


</p>

<hr>

<!-- <h1 id="headings">Headings</h1>

<h1>h1. Heading</h1>
<h2>h2. Heading</h2>
<h3>h3. Heading</h3>
<h4>h4. Heading</h4>
<h5>h5. Heading</h5>
<h6>h6. Heading</h6>

<hr>

<h1 id="paragraph">Paragraph</h1>

<p>Lorem ipsum dolor sit amet, <a href="#" title="test link">test link</a> adipiscing elit. Nullam dignissim convallis est. Quisque aliquam. Donec faucibus. Nunc iaculis suscipit dui. Nam sit amet sem. Aliquam libero nisi, imperdiet at, tincidunt nec, gravida vehicula, nisl. Praesent mattis, massa quis luctus fermentum, turpis mi volutpat justo, eu volutpat enim diam eget metus. Maecenas ornare tortor. Donec sed tellus eget sapien fringilla nonummy. Mauris a ante. Suspendisse quam sem, consequat at, commodo vitae, feugiat in, nunc. Morbi imperdiet augue quis tellus.</p>

<p>Lorem ipsum dolor sit amet, <em>emphasis</em> consectetuer adipiscing elit. Nullam dignissim convallis est. Quisque aliquam. Donec faucibus. Nunc iaculis suscipit dui. Nam sit amet sem. Aliquam libero nisi, imperdiet at, tincidunt nec, gravida vehicula, nisl. Praesent mattis, massa quis luctus fermentum, turpis mi volutpat justo, eu volutpat enim diam eget metus. Maecenas ornare tortor. Donec sed tellus eget sapien fringilla nonummy. Mauris a ante. Suspendisse quam sem, consequat at, commodo vitae, feugiat in, nunc. Morbi imperdiet augue quis tellus.</p>

<hr>

<h1 id="list_types">List Types</h1>

<p>Lists are unstyled by defualt. To restore the original styling, add the <code>.default</code> class</p>

<h3>Definition List</h3>
<dl>
  <dt>Definition List Title</dt>
  <dd>This is a definition list division.</dd>
</dl>

<h3>Ordered List</h3>
<ol>
  <li>List Item 1</li>
  <li>List Item 2</li>
  <li>List Item 3</li>
</ol>

<h3>Unordered List</h3>
<ul>
  <li>List Item 1</li>
  <li>List Item 2</li>
  <li>List Item 3</li>
</ul>

<h3>Ordered List with <code>.default</code> class</h3>
<ol class="default">
  <li>List Item 1</li>
  <li>List Item 2</li>
  <li>List Item 3</li>
</ol>

<h3>Unordered List with <code>.default</code> class</h3>
<ul class="default">
  <li>List Item 1</li>
  <li>List Item 2</li>
  <li>List Item 3</li>
</ul>

<hr>

<h1 id="form_elements">Fieldsets and Form Elements</h1>

<fieldset>
  <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Nullam dignissim convallis est. Quisque aliquam. Donec faucibus. Nunc iaculis suscipit dui. Nam sit amet sem. Aliquam libero nisi, imperdiet at, tincidunt nec, gravida vehicula, nisl. Praesent mattis, massa quis luctus fermentum, turpis mi volutpat justo, eu volutpat enim diam eget metus.</p>

  <form>
    <h2>Form Element</h2>

    <p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Nullam dignissim convallis est. Quisque aliquam. Donec faucibus. Nunc iaculis suscipit dui.</p>

    <p><label for="text_field">Text Field:</label>
      <input type="text" id="text_field" /></p>

    <p><label for="text_area">Text Area:</label>
      <textarea id="text_area"></textarea></p>

    <p><label for="select_element">Select Element:</label>
      <select name="select_element">
        <optgroup label="Option Group 1">
          <option value="1">Option 1</option>
          <option value="2">Option 2</option>
          <option value="3">Option 3</option>
        </optgroup>
        <optgroup label="Option Group 2">
          <option value="1">Option 1</option>
          <option value="2">Option 2</option>
          <option value="3">Option 3</option>
        </optgroup>
    </select></p>

    <p><label for="radio_buttons">Radio Buttons:</label>
      <label>
        <input type="radio" class="radio" name="radio_button" value="radio_1" /> Radio 1
      </label>
      <label>
        <input type="radio" class="radio" name="radio_button" value="radio_2" /> Radio 2
      </label>
      <label>
        <input type="radio" class="radio" name="radio_button" value="radio_3" /> Radio 3
      </label>
    </p>

    <p><label for="checkboxes">Checkboxes:</label>
      <label>
        <input type="checkbox" class="checkbox" name="checkboxes" value="check_1" /> Checkbox 1
      </label>
      <label>
        <input type="checkbox" class="checkbox" name="checkboxes" value="check_2" /> Checkbox 2
      </label>
      <label>
        <input type="checkbox" class="checkbox" name="checkboxes" value="check_3" /> Checkbox 3
      </label>
    </p>

    <p><label for="password">Password:</label>
      <input type="password" class="password" name="password" />
    </p>

    <p><label for="file">File Input:</label>
      <input type="file" class="file" name="file" />
    </p>


    <p><input type="submit" value="Submit" /></p>
  </form>
</fieldset>

<hr>

<h1 id="tables">Tables</h1>

<table cellspacing="0" cellpadding="0">
  <tr>
    <th>Table Header 1</th><th>Table Header 2</th><th>Table Header 3</th>
  </tr>
  <tr>
    <td>Division 1</td><td>Division 2</td><td>Division 3</td>
  </tr>
  <tr class="even">
    <td>Division 1</td><td>Division 2</td><td>Division 3</td>
  </tr>
  <tr>
    <td>Division 1</td><td>Division 2</td><td>Division 3</td>
  </tr>
</table> 
</div>-->
