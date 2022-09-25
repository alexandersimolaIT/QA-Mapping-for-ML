# QA-Mapping-for-ML
A mapping of existing literature in the field of ML testing. Helps in identifying relevant testing solutions given a context and testing goal. This repo contains results from our [Master's thesis][thesis]. There are two versions of this toolkit. Version 1 corresponds to the implementation we had before evaluating it by interviewing experts at a company, and version 2 is the improved implementation based on the feedback from the interviews.

## The Mapping Tool
The mapping tool can be found [here][mapping]. It is a table that can be filtered based on the tags in the different cells. Each row represents a paper that proposes a technique for testing ML systems. The columns represent different attributes of a paper, for example which testing goal is addressed, what type of testing technique is applied, or what ML task (e.g., classification, clustering, etc.) is being tested.

The tool is supported by five documents in this repo:
1. The Toolkit Guide ("toolkit_guide.pdf")
2. The Definitions document ("definitions.pdf")
3. The Goal Identification document ("goal_identification.pdf")
4. The Paper Summaries document ("paper_summaries.pdf")
5. Overview Tree Diagrams ("overview_trees.pdf")

## How to use the toolkit
A guide on how to use the mapping toolkit (tool + documents) can be found in "toolkit_guide.pdf".

## Definitions
This document ("definitions.pdf") contains definitions of all the tags used in the mapping tool. It contains one section for each column in the mapping, so that section then contains definitions for all of its tags. The point of this document is to clarify what each of the tags mean in this mapping, since the definitions in the literature sometimes differed from paper to paper.

## Goal Identification
This document ("goal_identification.pdf") seeks to help developers find what they need to be testing for. It contains a set of questions about the system to be tested, and if the developer answers yes to any of them then we suggest relevant testing goals. This document will mostly be useful for developers that don’t already know the quality attributes that they want to test their models for.

## Paper Summaries
This document ("paper_summaries.pdf") contains summaries of all papers in the mapping. Each paper has one paragraph that explains the proposed testing solution as well as some other relevant parts of the paper. The purpose of this document is to provide a glimpse into each paper so that developers can decide if the paper is relevant for them without fully reading the paper. However, if the paper does seem relevant to them, then it is encouraged to actually read the paper.

## Overview Tree Diagrams
These diagrams ("overview_trees.pdf") attempt to give an overview of what the mapping can offer in terms of testing techniques for different ML components.

Let's explain these diagrams... The green root node represents a component under test (CUT). This node is connected to red nodes that represent different testing goals (e.g., attributes like safety, fairness, robustness). These red nodes are connected to blue nodes that represent different types of testing techniques. All in all, each path from the root node to a leaf node (green -> red -> blue) means that there exists *at least one paper* in the mapping that proposes a solution for achieving the specified **testing goal** on the specific **CUT**  by applying a certain **type of testing**.

[mapping]: https://lists.live.com/:l:/g/personal/7caca96344176fc6/FH7iTutBDSFOqKiNJbDKkPsBJHO5TNue7vsSHfsg8e7XPQ
[thesis]: https://odr.chalmers.se/handle/20.500.12380/305129?locale=en
