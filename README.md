---
# The front matter describes the schema for the initial project.
# Remove the front matter in the actual project.

description: Configure flit for a single file project.
properties:
    name:
        type: string
        description: The name of the project
    description:
        type: string
        description: A short description for the project.

    author:
        type: string
        description: The name of the author
    email:
        type: string
        format: email
        description: The author's email
    packages:
        type: array
        description: A string of dependencies
    url:
        type: string
        format: uri
        description: The homepage for your project.

    license:
        type:
            enum:
            - Apache-2.0
            - BSD-2-Clause
            - BSD-3-Clause
            - BSD-4-Clause
            - GPL-2.0-only
            - GPL-2.0-or-later
            - GPL-3.0-only
            - GPL-3.0-or-later
            - LGPL-2.1-only
            - LGPL-2.1-or-later
            - LGPL-3.0-only
            - LGPL-3.0-or-later
            - MIT
        
---

# [{{name}}]({{url}})

> {{description}}

Written by [{{author}}]({{email}}) under a __{{license}}__ license.