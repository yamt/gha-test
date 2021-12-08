
a -> b

    https://docs.github.com/en/actions/learn-github-actions/reusing-workflows

    * can't rerun either "a" or "b" individually

a -> c

    https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows#workflow_run

    * "c" runs for the default branch
    * if you rerun "a", "c" is triggered each time

a -> d

    workflow_run + https://github.com/ahmadnassri/action-workflow-run-wait

    * "d" runs for the default branch
    * if you rerun "a", "d" is triggered each time
    * nicer handling of mutiple deps and their results
