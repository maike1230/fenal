# НОВАСТИ
## [заходи на сайт моих радителей](https://github.com/maike1230/-llo.git)
# НОВАСТИ РАССИИ
## [НО ПЕРЕД ПРЛЧТЕНИЕМ ЭТИХ НОВОСТЕЙ Я НОДЕЮСЬ ВЫ ОБРОТИЛИ ВНИМАНИЕ НА ЭТОТУ РЕКЛАМУ ЭТОТ САЙТ ВАМ ОЧЕНЬ ПОМОЖЕТ В ПРОДВИЖЕНИИ ВАШЕГО БИЗНАСА](https://www.google.ru/intl/ru_ru/adsense/start/?gclid=CjwKCAjw_ISWBhBkEiwAdqxb9jUEnILZyMZ1KPN7lqst72Hbiq6u62NHNNksVZU5-ZvAn5l4x_LJ2hoCIDgQAvD_BwE)
| ВАЛЮТА        | РУБЛЬ              | СОМ   |
| ------------- |:------------------:| -----:|
| ДОЛАР         | 57,00              | 79.50 |
| ЕВРО          | 59,45              |  82,91|
| ГРИВЕНЬ       | 1,93               |  2,69 |

![Иллюстрация к проекту](https://cdn.dribbble.com/users/24078/screenshots/14365732/24-01_4x.jpg)
<?php

class ChiefroomController extends Controller
{
    public $_metaTitle = 'Личный кабинет сотрудника';
    const IS_OPEN = TRUE;
    public $asUsers = array();
    /**
     * @var ASubordinate
     */
    public $asUser = NULL;
    private $segmentUserId = null;

    public function beforeAction($action)
    {
        $cssUrl = Yii::app()->assetManager->publish(Yii::getPathOfAlias('user.views.css'));
        Yii::app()->clientScript->registerCssFile($cssUrl.DIRECTORY_SEPARATOR.'chiefRoom.css');
        return true;
    }
