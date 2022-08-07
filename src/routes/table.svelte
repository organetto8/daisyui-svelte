<script lang="ts">

    import { Table, TableBody, TableData, TableHead, TableHeader, TableRow } from '$lib'

</script>

<Table>
    <TableHeader>
        <TableRow>
            <TableData>First Name</TableData>
            <TableData>Last Name</TableData>
            <TableData>Age</TableData>
        </TableRow>
    </TableHeader>
    <TableBody>
        <TableRow hover>
            <TableData>John</TableData>
            <TableData>Doe</TableData>
            <TableData>42</TableData>
        </TableRow>
        <TableRow hover>
            <TableData>Jane</TableData>
            <TableData>Doe</TableData>
            <TableData>39</TableData>
        </TableRow>
    </TableBody>
</Table>