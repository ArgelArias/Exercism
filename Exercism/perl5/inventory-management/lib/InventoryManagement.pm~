package InventoryManagement;

use v5.40;

sub create_inventory ($items) {
    my %inventory;
    map { $inventory{$_} = $inventory{$_} +1 } @$items;
    return \%inventory;
}

sub add_items ( $inventory, $items ) {
    map { $$inventory{$_} = $$inventory{$_} +1 } @$items;
    return $inventory;
}

sub remove_items ( $inventory, $items ) {
    map { ($$inventory{$_} > 0) ? ($$inventory{$_} = $$inventory{$_} -1 ) : ''  } @$items
    return $inventory;
}

sub delete_item ( $inventory, $item ) {
    delete($$inventory{$item});
    return $inventory;
}

1;
