---
layout: question-bank
---

<div class="bank-tabs" role="tablist" aria-label="Question bank" markdown="1">
  <input type="radio" name="bank" id="bank-basics" checked>
  <label for="bank-basics" role="tab">C++ Basics</label>

  <input type="radio" name="bank" id="bank-cpp1114">
  <label for="bank-cpp1114" role="tab">C++11/14</label>

  <div class="bank-panel bank-panel-basics" role="tabpanel" markdown="1">
{% include_relative cppbasicsquestion-bank.md %}
  </div>

  <div class="bank-panel bank-panel-cpp1114" role="tabpanel" markdown="1">
{% include_relative cpp1114question-bank.md %}
  </div>
</div>
