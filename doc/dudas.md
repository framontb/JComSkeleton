

# skeletons/joomprosubs/admin/views/submanager/tmpl/default.php

* Qué es JHtml?
* Para qué sirve el form.token?
```[PHP]
<?php echo JHtml::_('form.token'); ?>
```

# JoomprosubsHelper::getActions()

Sustituido por 
```
$canDo = JHelperContent::getActions('com_banners', 'category', $this->state->get('filter.category_id'));
```

Ver en `BannersViewBanners` como está hoy día.

# JoomprosubsViewSubmanager::addToolbar

* No se muestra NEW:
```
		if (count($user->getAuthorisedCategories('com_joomprosubs', 'core.create')) > 0)
		{
			JToolbarHelper::addNew('subscription.add','JTOOLBAR_NEW');
		}
```