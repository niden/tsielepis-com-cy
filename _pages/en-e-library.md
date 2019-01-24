---
layout: page_full
language: en
image: /assets/files/e-library.jpg
title: E-Library
permalink: /en/e-library
---
E-Library represents our digital repository of industry and tax information, guides, information sheets and more resources that maybe of real interest to you or your clients.

The proprietary information contained in the repository has been internally researched and developed and every reasonable effort was made to ensure its accuracy and timeliness. However, professional advice is always recommended before acting upon it.

The E-Library is constantly updated and enriched, therefore we urge you to come back often for new information.

<table id="e-library" class="display" style="width:100%">
    <thead>
        <tr>
            <th>Title</th>
            <th>Lang</th>
            <th>Type</th>
            <th>Date</th>
            <th>File</th>
        </tr>
    </thead>
    <tbody>
        {% for item in site.data.library.media %}
        <tr>
            <td>{{ item.title }}</td>
            <td>{{ item.language }}</td>
            <td>{{ item.types }}</td>
            <td>{{ item.date | date: "%B %Y" }}</td>
            <td><a href="{{ item.file }}">Download</a></td>
        </tr>
        {% endfor %}
    </tbody>
</table>