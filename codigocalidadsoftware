


<?xml version="1.0" encoding="utf-8" ?>
<ContentPage xmlns="http://schemas.microsoft.com/dotnet/2021/maui"
             xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml"
             x:Class="MenuAlmacenamiento.Views.ProductosPage"
             Title="Productos">
    <VerticalStackLayout Padding="10">
        <!-- Botón para agregar un nuevo producto -->
        <Button Text="Agregar Producto" Command="{Binding AgregarProductoCommand}" />

        <!-- Lista de productos -->
        <ListView x:Name="productosListView" 
                  ItemsSource="{Binding Productos}">
            <ListView.ItemTemplate>
                <DataTemplate>
                    <TextCell Text="{Binding Nombre}" 
                              Detail="{Binding Precio, StringFormat='Precio: {0:C}'}">
                        <TextCell.ContextActions>
                            <MenuItem Text="Editar" Command="{Binding BindingContext.EditarProductoCommand, Source={x:Reference productosListView}}" CommandParameter="{Binding .}" />
                            <MenuItem Text="Eliminar" Command="{Binding BindingContext.EliminarProductoCommand, Source={x:Reference productosListView}}" CommandParameter="{Binding .}" />
                        </TextCell.ContextActions>
                    </TextCell>
                </DataTemplate>
            </ListView.ItemTemplate>
        </ListView>
    </VerticalStackLayout>
</ContentPage>
