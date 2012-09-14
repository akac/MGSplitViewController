## MGSplitViewController for WebIS

This commit is my first commit of the changes we've made over the last year. Some of the changes are due to how WE use the code in our own project.
I've also removed all the sample code because we don't use. Only the class exists. Some of the changes include:

1. Added WebIS Copyright due to our changes. We're following Matt's original license however.
2. This uses our own Popover manager - you'll have to remove that to make this work. Again, this class was modified heavily to work within our own project. It is only being shared to help others.
3. We slide the master "popover" as in seen in the Mail app on iOS 5.1 and the normal split view on iOS 6
4. We've merged in some changes from other forks as well

## Usage

Instantiation is done as such (requires Xcode 4.5 and is supported on iOS 6 SDK - requires iOS 5 and above to work)
<pre><code>window.rootViewController = splitViewController;
[splitViewController setViewControllers:@[masterController,detailController]];
</code></pre>
