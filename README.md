RuleML2TPTP
=============================

*This is an easy-to-use translator utilizing XSLT 2.0 between two rule languages.*

### Introduction

[RuleML](http://wiki.ruleml.org) is a knowledge representation language developed by the non-profit organization RuleML Inc. RuleML is being used for sharing rule bases in XML and publishing them on the Web. It has broad coverage and is defined as an extensible family of sublanguages across various rule logics and platforms. RuleML consists of [Deliberation RuleML](http://wiki.ruleml.org/index.php/Specification_of_Deliberation_RuleML) and [Reaction RuleML](http://wiki.ruleml.org/index.php/Specification_of_Reaction_RuleML). 

This project is aimed at implementing an [XSLT 2.0](http://www.w3.org/TR/xslt20/) translator to convert [Datalog+](http://www.slideshare.net/polibear/datalog-and-its-extensions-for-semantic-web-databases) [Deliberation RuleML 1.01](http://wiki.ruleml.org/index.php/Specification_of_Deliberation_RuleML_1.01) in XML format to an equivalent representation in a subset of the (FOF) [TPTP](http://www.cs.miami.edu/~tptp/) language. See [here](http://deliberation.ruleml.org/1.01/doc/datalogplus_min_normal/) for the normalized Datalog+ Deliberation RuleML 1.01 schema on which this project is based.

The entry page of the project is [here](http://edmonl.github.io/RuleML2TPTP/).

### Getting Started

1. Download the binary or source code from the [project releases](https://github.com/EdmonL/RuleML2TPTP/releases).
2. If the source code is downloaded, use ant to build by "ant jar". See "ant -projecthelp" for other ant targets.
3. Translate a RuleML file by calling "java -jar /path/to/ruleml2tptp.jar -s &lt;source RuleML filename&gt; -o &lt;output filename&gt;". See "java -jar /path/to/ruleml2tptp.jar -h" for full usage.
4. Java SE 7 or higher is recommended.
5. Saxon is used dynamically, so saxon.jar can be removed and the local JAXP implementation will be used instead. Make sure, however, that the local implementation supports XSLT 2.0, or things will go wrong.
6. See the [project wiki](https://github.com/EdmonL/RuleML2TPTP/wiki) for other documentation.

### RuleML Examples

Here are some good RuleML examples from [RuleML wiki](http://wiki.ruleml.org/index.php/Specification_of_Deliberation_RuleML_1.01#Examples) or [here](http://deliberation.ruleml.org/1.01/exa/DatalogPlus/) to try with this project.

### License

This project is under [GNU GPL v3.0](https://github.com/EdmonL/RuleML2TPTP/blob/master/LICENSE).
