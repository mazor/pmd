---
title: Design
summary: Rules that help you discover design issues.
permalink: pmd_rules_vm_design.html
folder: pmd/rules/vm
sidebaractiveurl: /pmd_rules_vm.html
editmepath: ../pmd-vm/src/main/resources/category/vm/design.xml
keywords: Design, AvoidDeeplyNestedIfStmts, CollapsibleIfStatements, ExcessiveTemplateLength, NoInlineJavaScript, NoInlineStyles
---
## AvoidDeeplyNestedIfStmts

**Since:** PMD 5.1

**Priority:** Medium (3)

Avoid creating deeply nested if-then statements since they are harder to read and error-prone to maintain.

**This rule is defined by the following Java class:** [net.sourceforge.pmd.lang.vm.rule.design.AvoidDeeplyNestedIfStmtsRule](https://github.com/pmd/pmd/blob/master/pmd-vm/src/main/java/net/sourceforge/pmd/lang/vm/rule/design/AvoidDeeplyNestedIfStmtsRule.java)

**This rule has the following properties:**

|Name|Default Value|Description|
|----|-------------|-----------|
|problemDepth|3|The if statement depth reporting threshold|

**Use this rule by referencing it:**
``` xml
<rule ref="rulesets/vm/design.xml/AvoidDeeplyNestedIfStmts" />
```

## CollapsibleIfStatements

**Since:** PMD 5.1

**Priority:** Medium (3)

Sometimes two consecutive 'if' statements can be consolidated by separating their conditions with a boolean short-circuit operator.

**This rule is defined by the following Java class:** [net.sourceforge.pmd.lang.vm.rule.design.CollapsibleIfStatementsRule](https://github.com/pmd/pmd/blob/master/pmd-vm/src/main/java/net/sourceforge/pmd/lang/vm/rule/design/CollapsibleIfStatementsRule.java)

**Use this rule by referencing it:**
``` xml
<rule ref="rulesets/vm/design.xml/CollapsibleIfStatements" />
```

## ExcessiveTemplateLength

**Since:** PMD 5.1

**Priority:** Medium (3)

The template is too long. It should be broken up into smaller pieces.

**This rule is defined by the following Java class:** [net.sourceforge.pmd.lang.vm.rule.design.ExcessiveTemplateLengthRule](https://github.com/pmd/pmd/blob/master/pmd-vm/src/main/java/net/sourceforge/pmd/lang/vm/rule/design/ExcessiveTemplateLengthRule.java)

**This rule has the following properties:**

|Name|Default Value|Description|
|----|-------------|-----------|
|topscore||Top score value|
|minimum||Minimum reporting threshold|
|sigma||Sigma value|

**Use this rule by referencing it:**
``` xml
<rule ref="rulesets/vm/design.xml/ExcessiveTemplateLength" />
```

## NoInlineJavaScript

**Since:** PMD 5.1

**Priority:** Medium High (2)

Avoid inline JavaScript. Import .js files instead.

**This rule is defined by the following Java class:** [net.sourceforge.pmd.lang.vm.rule.design.NoInlineJavaScriptRule](https://github.com/pmd/pmd/blob/master/pmd-vm/src/main/java/net/sourceforge/pmd/lang/vm/rule/design/NoInlineJavaScriptRule.java)

**Use this rule by referencing it:**
``` xml
<rule ref="rulesets/vm/design.xml/NoInlineJavaScript" />
```

## NoInlineStyles

**Since:** PMD 5.1

**Priority:** Medium High (2)

Avoid inline styles. Use css classes instead.

```
//Text[matches(@literal, "<[^>]+\s[sS][tT][yY][lL][eE]\s*=")]
```

**Use this rule by referencing it:**
``` xml
<rule ref="rulesets/vm/design.xml/NoInlineStyles" />
```

