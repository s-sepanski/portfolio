# Welcome! My name is S. Sepanski

Career contributions over time (WIP):

## Color Key for Nodes

Todo

## Label Key for Relationships

- **then**: Indicates the passage of time between events.
- **unlabeled**: This connection is either invalid or in draft status.

## Key for Node Content

- **@**: Indicates having joined or completed work associated with a particular company or organization.
- **Level**: Software engineer level, normalized to L1-L10, as described by [this LinkedIn post](https://www.linkedin.com/pulse/understanding-software-engineer-levels-from-entry-level-senior-pke9c/) (L1-L5) and [levels.fyi](https://www.levels.fyi/blog/swe-level-framework.html) (L6-L10)

## About Node Content

- **Dates**:
  - Formats like **YYYY** indicate that the node transpired for an unspecified duration in the given calendar year
  - Formats like **YYYY-YYYY** indicate that the node transpired for an unspecified duration within the given year range

```mermaid
graph TD
    PreStudentNode["<div style='font-size:75%;  color:#848484; text-align:center;'>2015-2020</div>Student"] -->|then| A["<div style='font-size:75%; color:#848484; text-align:center;'>2020</div><div style='font-size:75%; color:#848484; text-align:center;'><b>Level: L2</b><br/></div>Joined @USAA<br>"]
    ContractorNode["<div style='font-size:75%; color:#848484; text-align:center;'>2018-2020</div><div style='font-size:75%; color:#848484; text-align:center;'><b>Level: L1</b></div>Intern/Contractor"] -->|then| A
    A -->|then| B["<div style='font-size:75%; color:#848484; text-align:center;'>YYYY</div>todo"]
    B -->|then| C["<div style='font-size:75%; color:#848484; text-align:center;'>2025</div><div style='font-size:75%; color:#848484; text-align:center;'><b>Level: L3</b><br/></div><SWE 1 2025<br>• Gave talk to 200-odd people in dev community (hosted by Bank Deposits department yet shared enterprise-wide) on GitHub Copilot in collaboration w/ L. Ortin (spoke for second half of hour)<br>• Item 2<br>• Item 3"]
    C -->|then| D["<div style='font-size:75%; color:#848484; text-align:center;'>YYYY</div>todo"]
    B -->|then| E["<div style='font-size:75%; color:#848484; text-align:center;'>YYYY</div>Achievement 1"]
    C -->|then| F["<div style='font-size:75%; color:#848484; text-align:center;'>YYYY</div>Achievement 2"]
    D -->|then| G["<div style='font-size:75%; color:#848484; text-align:center;'>YYYY</div>Achievement 3"]
    style PreStudentNode fill:#e5e5e5,stroke:#343434,stroke-width:2px,color:#1c1c1c
    style ContractorNode fill:#e5e5e5,stroke:#343434,stroke-width:2px,color:#1c1c1c
    style A fill:#f58e9f,stroke:#610b2f,stroke-width:2px,color:#230519
    style B fill:#e5e5e5,stroke:#343434,stroke-width:2px,color:#1c1c1c
    style C fill:#d1193e,stroke:#610b2f,stroke-width:2px,color:#FFFFFF
    style D fill:#042748,stroke:#042e5c,stroke-width:2px,color:#FFFFFF
    style E fill:#c2c2c2,stroke:#343434,stroke-width:2px,color:#1c1c1c
    style F fill:#c2c2c2,stroke:#343434,stroke-width:2px,color:#1c1c1c
    style G fill:#c2c2c2,stroke:#343434,stroke-width:2px,color:#1c1c1c
    classDef rounded stroke-width:2px,rx:10,ry:10;
    class PreStudentNode,ContractorNode,A,B,C,D,E,F,G rounded;
```

# Coding Standards for This Project

- This project aims to follow [semantic commit messages](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716), electing to make the following modifications:
  - Substitute the word `task:` for `chore:` because it has a slightly more positive connotation.
  - Add a new category:
    - `wip`: (work in progress, a commit that really should be squashed. Most likely made to save changes because I had to go afk due to some happenstance of life)
