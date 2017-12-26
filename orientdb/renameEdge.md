    alter class OWNS name DRIVES

    UPDATE V SET out_DRIVES = out_OWNS where out_OWNS is not null

    UPDATE V SET in_DRIVES = in_OWNS where in_OWNS is not null

    UPDATE V REMOVE out_OWNS where out_OWNS is not null
    UPDATE V REMOVE in_OWNS where in_OWNS is not null
