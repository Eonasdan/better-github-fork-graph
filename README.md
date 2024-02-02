 <p>
                I hate using the GitHub network graph. It's too difficult to find any useful changes from other forks. I made this little tool to make it easier. It does this by filtering out forks and commits that have no changes from the base repo.
            </p>
            <p>
                Provide a repo like `owner/repo` (required).
            </p>
            <p>
                You can optionally provide a date that you want to limit commits to. If provided, any commits that occurred before this date will not be requested by the API call.
            </p>
            <p>
                If you select "Use Last Commit Date", then the last commit from the provided repo will be used automatically.
            </p>
            <p>
                If you select "Load All", then the app will get all the forks, branches and commits at one time. Otherwise, it will only load the forks you click on. Note, that in this mode, it won't filter out commits with the same hash. This does take some time, depending on the number of forks there are.
            </p>
            <p>
                Lastly, I know it's weird, but the app usually
                <a href="https://github.com/settings/tokens?type=beta"
                   target="_blank"
                   rel="noopener">
                    needs a PAT
                </a>.
                You can try it without, but it will likely hit the API limit. There isn't a good way to use the OAuth flow without exposing a secret. All this is used for is calling the API. I don't store, or use it for anything else. There's no tracking of any kind. You are welcome to review
                <a href="https://github.com/Eonasdan/better-github-fork-graph"
                   target="_blank"
                   rel="noopener">
                    the app source code
                </a>
                or run it locally if you wish.
            </p>