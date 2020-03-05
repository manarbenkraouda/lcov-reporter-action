# Jest reporter action

This action comments a pull request with a HTML test coverage report.

The report is based on the lcov coverage report generated by your test runner.

Note that this action does not run any tests, but instead expects the tests to have been run
by another action already.

## Example output

Total Coverage: <b>99.39%</b>

<details><summary>Coverage Report</summary><table><tbody><tr><th>File</th><th>Branches</th><th>Funcs</th><th>Lines</th><th>Uncovered Lines</th></tr><tr><td colspan='5'><b>src</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/i18n.tsx'>i18n.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/i18n</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/i18n/context.tsx'>context.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/i18n/hydrate.tsx'>hydrate.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/i18n/index.tsx'>index.tsx</a></td><td><b>85.71%</b></td><td><b>88.89%</b></td><td>100%</td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/i18n/index.tsx#L54'>54</a></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/i18n/link.tsx'>link.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/icon</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/icon/index.tsx'>index.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/icon/props.tsx'>props.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/layout</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/layout/index.tsx'>index.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/release-artist-link</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-artist-link/index.tsx'>index.tsx</a></td><td><b>66.67%</b></td><td>100%</td><td>100%</td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-artist-link/index.tsx#L24'>24</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-artist-link/index.tsx#L25'>25</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-artist-link/index.tsx#L26'>26</a></td></tr><tr><td colspan='5'><b>src/components/release-companies</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-companies/index.tsx'>index.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/release-credits</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-credits/index.tsx'>index.tsx</a></td><td><b>85.71%</b></td><td>100%</td><td><b>91.30%</b></td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-credits/index.tsx#L37'>37</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-credits/index.tsx#L38'>38</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-credits/index.tsx#L40'>40</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-credits/index.tsx#L43'>43</a></td></tr><tr><td colspan='5'><b>src/components/release-format-link</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-format-link/index.tsx'>index.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/release-header</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-header/index.tsx'>index.tsx</a></td><td><b>58.33%</b></td><td>100%</td><td>100%</td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-header/index.tsx#L79'>79</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-header/index.tsx#L80'>80</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-header/index.tsx#L82'>82</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-header/index.tsx#L85'>85</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-header/index.tsx#L86'>86</a></td></tr><tr><td colspan='5'><b>src/components/release-label-link</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-label-link/index.tsx'>index.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/components/release-series-link</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-series-link/index.tsx'>index.tsx</a></td><td><b>0%</b></td><td>100%</td><td>100%</td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-series-link/index.tsx#L19'>19</a></td></tr><tr><td colspan='5'><b>src/components/release-thumbnail</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-thumbnail/icon.tsx'>icon.tsx</a></td><td><b>50%</b></td><td>100%</td><td><b>83.33%</b></td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-thumbnail/icon.tsx#L26'>26</a>, <a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-thumbnail/icon.tsx#L30'>30</a></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-thumbnail/index.tsx'>index.tsx</a></td><td><b>75%</b></td><td>100%</td><td>100%</td><td><a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/release-thumbnail/index.tsx#L42'>42</a></td></tr><tr><td colspan='5'><b>src/components/search</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/search/index.tsx'>index.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/search/mock.tsx'>mock.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/components/search/ui.tsx'>ui.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/lib</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/lib/add-state.tsx'>add-state.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/lib/intersperse.tsx'>intersperse.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/lib/keycodes.tsx'>keycodes.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/lib/slug.tsx'>slug.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr><tr><td colspan='5'><b>src/services</b></td></tr><tr><td>&nbsp; &nbsp;<a href='https://github.com/example/foo/blob/f9d42291812ed03bb197e48050ac38ac6befe4e5/src/services/autocomplete.tsx'>autocomplete.tsx</a></td><td>100%</td><td>100%</td><td>100%</td><td></td></tr></tbody></table></details>

## Inputs

##### `github-token` (**Required**)
Github token used for posting the comment. To use the key provided by the GitHub
action runner, use `${{ secrets.GITHUB_TOKEN }}`.

##### `lcov-file` (**Optional**)
The location of the lcov file to read the coverage report from. Defaults to
`./coverage/lcov.info`.

##### `lcov-base` (**Optional**)
The location of the lcov file resulting from running the tests in the base
branch. When this is set a diff of the coverage percentages is shown.

## Example usage

```yml
uses: romeovs/lcov-reporter-action@v0.2.16
with:
  github-token: ${{ secrets.GITHUB_TOKEN }}
  lcov-file: ./coverage/lcov.info
```

## Acknowledgements

The initial code is based on [ziishaned/jest-reporter-action](https://github.com/ziishaned/jest-reporter-action).
