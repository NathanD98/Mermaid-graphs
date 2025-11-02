gitGraph
    commit id: "Initial commit"
    branch develop
    checkout develop
    commit id: "Develop setup"
    branch feature
    checkout feature
    commit id: "Feature work 1"
    commit id: "Feature work 2"
    checkout develop
    merge feature id: "Merge feature into develop"
    branch release
    checkout release
    commit id: "Release prep"
    checkout main
    merge release id: "Merge release into main"
    checkout develop