# Will it GoCD?

[![Build Status](https://travis-ci.org/d-led/will_it_go_cd.svg?branch=master)](https://travis-ci.org/d-led/will_it_go_cd) [![Build status](https://ci.appveyor.com/api/projects/status/bdhlyf1x1aij6c6u/branch/master?svg=true)](https://ci.appveyor.com/project/d-led/will-it-go-cd/branch/master)

> This is a little [GoCD](https://www.gocd.org) configuration analysis and audit helper tool

## Motivation

GoCD is a very user friendly and sophisticated Continuous Integration / Continuous Delivery tool. GoCD allows gradual immersion in its features by means of sensible defaults and a very well documented [concept language](https://docs.gocd.org/current/introduction/concepts_in_go.html). When many features of GoCD are used, it is easy to overlook misconfigured pipelines, e.g. when there is no agent with the resource required by a job, or when a pipeline is not part of the environment, where the dedicated agent is configured. This tool should give a quick overview of certain aspects of the configuration

## Current Queries

- what agents are there and how are they configured? Summary, as it's already part of the GoCD UI.
- misconfigured agents: which jobs can an agent potentially run?
- capacity planning and misconfigured jobs: which agents can a job run on?

## Guarantees

- **None**
- **No guarantees of fitness for any kind of task**, use at your own risk

## Rough Plan

contributions with new analyses are welcome!

- apply parameter interpolation
- expand pipeline templates (good first issue)
- get the configuration from a URL (good first issue)
- get pipeline config from remote pipeline-as-code repos
