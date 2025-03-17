# MarkPub Upgrade Notes  

Notes on steps taken and on breakdowns and resolutions of problems
encountered. (2025-03-16: WLA the primary dev on this)  

- branch "wla-markpub-upgrade-20250316" created to hold and test the
  changes needed for the upgrade.  
  
- first phase steps:
  - insure MWB works on this branch  
  
  - initialize this branch with `markpub` files  
  
  - insure that this branch works using `markpub`  
  - get review from Jerry and Pete  
  
### 2025-03-17 notes:    

- DONE: `markpub init`  
  (copied the GitHub link info from `mwb.yaml`)  

- first local build (without --lunr or --commits) 
- DONE: combine `Sidebar.md` and `Sidebar-new.mf`  

- DONE: turned on lunr

- BREAKDOWN: `.github/workflows` did not get installed; why?  
  TODO: manually install the workflow  
  RESOLUTION:  
  - i did not find a way to run the MarkPub gh-pages.yml file and
    indicate to GitHub Pages to use `gh-pages` as the branch from the
    markpub-update branch.  
  - workaround: deploy the markpub-upate branch with netlify to this
    URL: <https://mptest-ogmwiki.netlify.app/>  


	
  

