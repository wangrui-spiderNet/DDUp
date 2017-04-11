# DDUp
DDUP设计
前身
巨变
秘密
转化


主线：
科技危机，科技的生长脱离的多数人的掌控后

更先进不代表更强大

副线：
科技的发展对人类社会的巨大影响，科技的残酷，不同阶层人类面对巨变的命运
人类对自由的渴求，对永生的渴求，对成为神的渴求
人没有善恶，只是立场处境不同而已
生命的意义到底为何?
真实的人工智能到底是会怎么样？
政府的角色？
科技竞赛如果脱离了政府的掌控？
高科技公司的演变
战争还是和平？
不能调和的矛盾
越来越大的差距
富者永生，穷者无助
时间的不平等
身体的差异
高等级的人与低等级的人
如何重新定义人
不能改变的现实-人性（自私，欲望，绝对自由，绝对的孤独，无上的权力，恐惧）
暂时的困境
过渡期会怎么样发生？
新的世界会如何到来？
人类的潜力到底有没有边界？
进化的代价
得到什么，失去什么？
科技的原始驱动力是什么？邪恶还是好奇？欲望和懒惰还是聪明的大脑
一切都在改变，唯有人性未变
选择
更“好”的人，普通人？
改变了的人性还是人吗？

智人和半超人


剧情转换：
巨变，重生，进化，新的朋友，两种人，另一个世界，阴谋，背后的背后，巨变，
逃离，变强，自由，责任，路在何方


主要情绪：
科技的冰冷
无助
恐惧
残酷
邪恶
金钱
战争
交易
力量
兴奋
亲情
抚慰
自由


原则：
大胆猜测，仔细构想

像在讲述过去一样讲述未来

先想象一下一百年以后会是怎么样一个社会，然后倒退从现在走向未来100年中间会发生什么

满足普通人对未来的窥探，对科技发展的好奇

===========================================================================
智远集团首席科学家  王安  他的儿子 王栩然 小天才

故事主线：
第一部分：
平静的生活突然有一天出现了崩塌，全家失散，城市陷落，人们流离失所，只有自己的小机器人还在身边陪伴，为了弄清楚这到底是怎么回事，找到父母，主人公开始一段探索，随着探索的深入揭露出了一个惊人的秘密，原来这一切的发生都不是突然发生的，一个超级庞大和黑暗的组织开始出现，主人公开始了一段与超级巨鳄斗争之旅。


第二部分：
当超级巨额的面目一步步更加清晰的时候，一个更大的阴谋和谎言开始出现，他的父母的身份让人怀疑，他自己又是谁？
他只是一对科学家（他的父母）的研究成果而已，而过去的种种也只是整个实验的一部分，真实的世界远不是这样。他该怎么办，按照设定的命运走向垃圾场，还是争取自己的生存权利？在父母的帮助下，他活了下来。
他，一个机器人，被人类创造出来的人，面对人类的设定会做出什么样的选择？他超乎普通人类的能力在面对脆弱的真实人类的时候，当他已经主宰了自己的命运，还有能力主宰全人类的命运的时候，他会怎么做？


第三部分：这只是一个实验。

实验的完整版图
第一阶段：培养
第二阶段：接受考验，判别是非的能力测试，面对恶劣的环境的生存能力测试
第三阶段：探索真相，接受现实，精准的反抗测试，当接受自己是机器人之后，他要为了生存而抗争，当经受人类的摧残和恶意，生存下来并强大之后，能够依然保持对人类和世界的热爱。
第四阶段：实验结束，实验结论，机器人是可信的，通过测试，可以批量生产进入人类社会。


第四部分：觉醒。

1、adb logcat 　　　　　　　　  --打印当前设备上所有日志

2、adb logcat | findstr ***　　 --过滤仅含***的日志

3、adb logcat *:W 　　　　　　 --过滤打印严重级别W及以上的日志

4、adb logcat | findstr *** > F:\log.txt 　　 --把仅含***的日志保存到F盘的log.txt文件中

5、adb logcat -c 　　　　　　    -- 清除屏幕上的日志记录

6、adb logcat -c && adb logcat -s ActivityManager | grep "Displayed”  　　--客户端程序启动时间获取

查看当前Activity
Windows :
adb shell dumpsys activity | find "mFocused"

MAC:
adb shell dumpsys activity | grep mFocused 


cmd常用控制台
1、清屏命令：cls
2、列出当前目录详细信息：dir
3、删除文件：del xxx.txt


android adb常用命令
1)、创建sdcard
mksdcard 50M D:/sdcard.img --> 创建一张容量为50M的SDCard

2)、删除sdcard
cd d:/
del sdcard.img

3)、把ljq.txt文件放在sdcard
adb push d:/ljq.txt /sdcard/

4)、创建avd模拟器
android create avd -n avd名称 -t target平台编号
eg、android create avd -n android2.1 -t 8

说明：Error: Folder C:\Users\Administrator\.android\avd\ljq.avd is in the way. Use --f
orce if you want to overwrite.(进入C:\Users\Administrator\.android\avd\目录，把ljq.avd文件夹删除即可)

5)、启动模拟器
emulator -avd xxx
eg、emulator -avd android2.1
启动带sdcard模拟器
emulator -sdcard d:/sd.img -avd android2.1(android2.1之前创建好的一个虚拟设备的名称)

6)、删除AVD（模拟器）：
android delete avd -n name名称
eg、android delete avd -n android2.1

7)、显示系统中全部android平台
android list targets

8)、android list avd 

9)、adb devices

10)、查看用户已安装的软件
adb shell
cd /data/app/ 
ls

11)、安装软件
adb install d:\abc.apk

12)、卸载软件
adb shell
cd /data/app/
adb uninstall <软件名> 
adb uninstall -k <软件名> 
说明：如果加 -k 参数,为卸载软件但是保留配置和缓存文件. </B>
eg、adb uninstall com.ljq.activity

13)、启动ddms：ddms

14)、导出文件
adb pull adb pull <远程路径> <本地路径>  
eg、adb pull /sdcard/hrtx/123.gif d:/

15)、导入文件
adb push <本地路径> <远程路径>
eg、adb pull d:/123.gif /sdcard/

16)、进入模拟器的shell模式：
adb shell

17)、在命令行中查看LOG信息：
adb logcat
adb logcat -s 标签名
eg、adb logcat -s MainActivity

18)、删除系统应用：
adb remount(重新挂载系统分区，使系统分区重新可写)
adb shell
cd /system/app
rm *.apk

19)、获取管理员权限：
adb root

20)、启动Activity
adb shell am start -n 包名/包名＋类名(-n 类名,-a action,-d date,-m MIME-TYPE,-c category,-e 扩展数据,等)
eg、adb shell am start -n com.hrtx.activity/com.hrtx.activity.MainActivity

21)、发布端口： 
设置任意的端口号，做为主机向模拟器或设备的请求端口。
eg、adb forward tcp:5555 tcp:8000 

22)、查看bug报告： 
adb bugreport 

23)、记录无线通讯日志： 
一般来说，无线通讯的日志非常多，在运行时没必要去记录，但我们还是可以通过命令设置记录： 
adb shell 
logcat -b radio 

24)、获取设备的ID和序列号： 
adb get-product 
adb get-serialno 

25)、访问数据库SQLite3 
adb shell 
sqlite

==================================================================================================================================

package com.android.clientApp;

//客户端代码  关键代码 导包.java
import com.example.android.testapp.aidl.IRequestCallBack;
import com.example.android.testapp.aidl.IRequestCityWeather;
import com.example.android.testapp.aidl.RequestData;
import com.android.clientApp.weather.WeatherParseJson;

public class EventInfoFragment extends Fragment {
    

    // This is currently required by the fragment manager.
    public EventInfoFragment() {
    }
   
    @Override
    public void onActivityCreated(Bundle savedInstanceState) {
        super.onActivityCreated(savedInstanceState);
        mContext = getActivity();
    }
   
    public void onAttach(Activity activity) {
        super.onAttach(activity);
        //关键代码
       
        bindAIDLService();
       
   
    }

    public View onCreateView(LayoutInflater inflater, ViewGroup container, Bundle savedInstanceState) {
        Log.e(TAG, "fx---->onCreateView: " );
        //... 加载VIEW的过程

        return mView;
    }

  
    @Override
    public void onDestroyView() {
        // 注销  关键代码
        getActivity().unbindService(mWeatherSeriveConnection);
       
        super.onDestroyView();
    }

    @Override
    public void onDestroy() {
       
        // System.gc();
    }

	//关键代码
    private void bindAIDLService() {
        try {
            Log.e(TAG, "fx---->bindAIDLService: " );
            Intent intent = new Intent();
            intent.setComponent(new ComponentName("com.example.android.testapp", 

"com.example.android.testapp.aidl.WeatherAidlService"));//这两个参数，第一个是server APP的包名，第二个是AIDLService包名路径
            boolean bindResult = getActivity().bindService(intent, mWeatherSeriveConnection, Context.BIND_AUTO_CREATE);
            Log.e(TAG, "fx---->bindResult : " + bindResult);
            mTitle.setText("fx---->= " + bindResult, BufferType.SPANNABLE);

        } catch (Exception e) {
            Log.e(TAG, "fx--->bindService Exception, " + e.toString());
        }

    }
    

    private IRequestCityWeather requestCityWeather = null;


	//关键代码
    private final ServiceConnection mWeatherSeriveConnection = new ServiceConnection() {

        @Override
        public void onServiceDisconnected(ComponentName name) {
            
            try {
                Log.e(TAG, "fx---->EventInfoFragment onServiceDisconnected PackageName : " + getActivity().getPackageName());
                requestCityWeather.unregisterCallBack(mCallBack, getActivity().getPackageName());
            } catch (RemoteException e) {
                Log.e(TAG, "fx---->onServiceDisconnected RemoteException : " + e.getMessage());
            }
            requestCityWeather = null;
        }

		
        @Override
        public void onServiceConnected(ComponentName name, IBinder service) {
            // TODO Auto-generated method stub
            Log.e(TAG, "fx---->onServiceConnected : " + name);
            if (service.isBinderAlive()) {
                Log.e(TAG, "fx---->onServiceConnected isBinderAlive:  " + service.isBinderAlive());
            } else {
                Log.e(TAG, "fx---->onServiceConnected isBinderAlive: " + service.isBinderAlive());
            }
            try {
                requestCityWeather = IRequestCityWeather.Stub.asInterface(service);
                Log.e(TAG, "fx----> onServiceConnected requestCityWeather to 3 -->" + requestCityWeather);

                if(requestCityWeather!=null){
                    registerCallBack();
                }else{
                    bindAIDLService();
                }
                
            } catch (NoSuchMethodError e) {
                Log.e(TAG, "fx---->onServiceConnected NoSuchMethodError : " + e.getMessage());
            } catch (Exception e) {
                Log.e(TAG, "fx---->onServiceConnected Exception : " + e.getMessage());
            }
        }
    };

	//关键代码
    private void registerCallBack() {

        try {
            Log.e(TAG, "fx---->registerCallBack to : requestCityWeather" + requestCityWeather);
            Log.e(TAG, "fx---->registerCallBack to : mCallBack" + mCallBack);
            
            requestCityWeather.registerCallBack(mCallBack, "com.android.clientApp");//注意第二个参数是clientAPP 的包名直接用 

getActivity().getPackageName()；这种方式更好
            
			
            requestDataByLocaiton(latitude, longitude, true);
            
        } catch (RemoteException e) {
            Log.e(TAG, "fx---->registerCallBack RemoteException : " + e.getMessage());
        }
    }

	//关键代码
    public IRequestCallBack.Stub mCallBack = new IRequestCallBack.Stub() {

        @Override
        public void onRequestResult(String weatherJsonData, RequestData requestData) throws RemoteException {
            Log.e(TAG, "fx---->EventInfoFragment onRequestResult requestFlag = " + requestData);
            Log.e(TAG, "fx---->EventInfoFragment weatherJsonData = " + weatherJsonData.toString());//打印从server APP返回的值
           // mWeather.setText();
            if (!TextUtils.isEmpty(weatherJsonData)) {
                showWeatherInfo(weatherJsonData,0);
            }

        }
    };

    private void requestDataByLocaiton(final double latitude, final double longitude, final boolean allDay) {
        Log.e(TAG, "fx---->requestDataByLocaiton latitude = to 5 " + latitude + ",longitude=" + longitude + ",allDay =" + 

allDay);
        if (null != requestCityWeather) {
            try {
                RequestData data = new RequestData(getActivity(), latitude, longitude);
                data.setmAllDay(allDay);
                requestCityWeather.requestWeatherByLocation(data);
                Log.e(TAG, "fx---->requestDataByLocaiton RequestData == " + data.toString());
            } catch (Exception e) {
                Log.e(TAG, "fx---->requestDataByLocaiton Exception " + e.toString());
            }
        } else {
            Log.e(TAG, "fx---->mCityWeatherManager null  end 6");
        }
    }

}

////////////////////////////////////////////////
package com.huawei.android.totemweather.aidl;
// 客户端/服务器端代码 AIDL文件 文件路径必须和服务端一致.aidl
import com.huawei.android.totemweather.aidl.RequestData;

interface IRequestCallBack {
    /** 
      * @param weatherJsonData Return the form of JSON data 
      * @param requestFlag 
      */
    void onRequestResult(String weatherJsonData, inout RequestData requestData);

}
/////////////////////////////////
// 客户端/服务器端代码 AIDL文件 文件路径必须和服务端一致.aidl
package com.huawei.android.totemweather.aidl;

import com.huawei.android.totemweather.aidl.IRequestCallBack;
import com.huawei.android.totemweather.aidl.RequestData;

interface IRequestCityWeather {

    /** 
      * request weather by the latitude and longitude,return the form of JSON data 
      * @param requestData RequestData
      * @return
      */
    void requestWeatherByLocation(in RequestData requestData);

     /** 
      * request the weather of cityInfo by the cityId from weather app.
      * @param requestData RequestData
      * @return 
      */
    void requestWeatherByCityId(in RequestData requestData);

    /** 
      * Get the weather of cityInfo by the cityType from weather app.
      * @param requestData RequestData
      * @return String Return the form of JSON data 
      */
    void getWeatherByType(in RequestData requestData);

    void registerCallBack(IRequestCallBack callback, String packageName);
    void unregisterCallBack(IRequestCallBack callback, String packageName);

    void requestWeatherByLocationAndSourceType(in RequestData requestData, int type);

    void requestWeatherWithLocation(in RequestData requestData, int sourceType, int parsePhaseType);
}

/////////////////////////////////
// 客户端/服务器端代码 AIDL文件 文件路径必须和服务端一致.aidl
package com.huawei.android.totemweather.aidl;

parcelable RequestData;

///////////////////////////////////////

// 服务器端代码 AIDL文件 文件路径必须和服务端一致.java
package com.example.android.testapp.aidl;

import java.util.HashMap;

import android.app.Service;
import android.content.Context;
import android.content.Intent;
import android.os.AsyncTask;
import android.os.IBinder;
import android.os.RemoteException;
import android.text.TextUtils;
import android.util.Log;

import com.example.android.testapp.controller.WeatherDataManager;
import com.example.android.testapp.controller.WeatherTaskController;
import com.example.android.testapp.controller.WeatherTaskInfo;
import com.example.android.testapp.location.HwLocationManager;
import com.example.android.testapp.location.HwLocationManager.LocationResult;
import com.example.android.testapp.location.TotemLocation;
import com.example.android.testapp.provider.BaseInfoUtils;
import com.example.android.testapp.provider.CityInfo;
import com.example.android.testapp.provider.Weather.WeatherInfo;
import com.example.android.testapp.provider.WeatherAlarm;
import com.example.android.testapp.utils.HomeCityWeather;
import com.example.android.testapp.utils.HwLog;
import com.example.android.testapp.utils.Utils;

public class WeatherAidlService extends Service {

    public static final String TAG = "WeatherAidlService";
    /** parse error result */
    public static final String PARSE_ERROR_RESULT = "";
    /** request result */
    public static final String REQUEST_RESULT = "request_result";
    /** request data */
    public static final String REQUEST_DATA = "request_data";

    private static final String THIRD_REQUEST_PERMISSION = "com.example.testapp.permission.THIRD_REQUEST_WEATHER";

    /** all application of register callback */
    public final HashMap<String, IRequestCallBack> mCallbackList = new HashMap<String, IRequestCallBack>();
    private WeatherDataManager mWeatherDataManager;

    @Override
    public void onCreate() {
        HwLog.d(TAG, "onCreate");
        mWeatherDataManager = WeatherDataManager.getInstance(this);
        Log.e(TAG, "fx---->WeatherAidlService onCreate");
        super.onCreate();
    }

    @Override
    public IBinder onBind(Intent intent) {
        HwLog.d(TAG, "onBind");     Log.e(TAG, "fx---->WeatherAidlService onBind");
        return mCityWeatherManager;
    }

    @Override
    public void onDestroy() {
        HwLog.d(TAG, "onDestroy");
        Log.e(TAG, "fx---->WeatherAidlService onDestroy");
        mCallbackList.clear();
        super.onDestroy();
    }

    public IRequestCityWeather.Stub mCityWeatherManager = new IRequestCityWeather.Stub() {

        @Override
        public void requestWeatherByLocation(RequestData requestData) throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            HwLog.d(TAG, "requestWeatherByLocation->enter");
            Log.e(TAG, "fx---->WeatherAidlService requestWeatherByLocation  requestData =="+requestData.toString());
            Log.e(TAG, "fx---->WeatherAidlService isRequestDataWithGeoPosInValidate::: "+isRequestDataWithGeoPosInValidate(requestData));
            if (isRequestDataWithGeoPosInValidate(requestData)) {
                HwLog.w(TAG, "requestWeatherByLocation->requestData with geo-position is invalidate");
                sendParseResult(requestData, PARSE_ERROR_RESULT);
                return;
            }

            WeatherAsyncTask task = new WeatherAsyncTask(requestData);
            Log.e(TAG, "fx---->WeatherAidlService task:: "+task.toString());
            task.execute(createWeatherTaskInfoBasedOnRequest(requestData));
        }

        @Override
        public void requestWeatherByCityId(RequestData requestData) throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            HwLog.d(TAG, "requestByCityId requestData = " + requestData);
            Log.e(TAG, "fx---->WeatherAidlService requestWeatherByCityId"+requestData.toString());
            if (null == requestData || TextUtils.isEmpty(requestData.getmCityId())
                    || !requestData.getmCityId().startsWith("cityId:")) {
                HwLog.w(TAG, "requestByCityId Exception : data=" + requestData);
                sendParseResult(requestData, PARSE_ERROR_RESULT);
                return;
            }
            CityInfo cityInfo = new CityInfo();
            BaseInfoUtils.setCityCode(cityInfo, requestData.getmCityId());
            WeatherTaskInfo info = new WeatherTaskInfo(cityInfo);
            //Log.i(TAG, " info " + info );/for test
            info.setTaskState(WeatherTaskInfo.WEATHER_TASK_INIT);
            WeatherAsyncTask task = new WeatherAsyncTask(requestData);
            task.execute(info);
        }

        @Override
        public void getWeatherByType(RequestData requestData) throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            HwLog.d(TAG, "requestByType requestData = " + requestData);
            Log.e(TAG, "fx---->WeatherAidlService getWeatherByType"+requestData.toString());
            if (null == requestData) {
                HwLog.d(TAG, "getWeatherByType requestData = null");
                requestData = new RequestData();
            }
            CityInfo cityInfo = null;
            WeatherInfo weatherInfo = null;
            switch (requestData.getmCityType()) {
            case RequestData.TYPE_MY_LOCATION:
                // request my location weather if exist
                cityInfo = queryLocationCityInfo();
                break;
            case RequestData.TYPE_HOME_CITY:
                // default home city
                cityInfo = Utils.getWidgetShowCityInfo(WeatherAidlService.this);
                    break;
            case RequestData.TYPE_HOME_CITY_FIRST:
                    // first return home city, return my location if home city not exists
                cityInfo = getHomeCityOrMyLocation();
                break;
            case RequestData.TYPE_MY_LOCATION_FIRST:
                // first return my location, return home city if my location not exists
                cityInfo = getMyLocationOrHomeCity();
                break;
            default:
                break;
            }

            if (null != cityInfo) {
                weatherInfo = queryWeatherInfo(cityInfo);
            }
            String jsonDataString = HomeCityWeather.packJsonData(WeatherAidlService.this, cityInfo,
                    weatherInfo, requestData.ismAllDay(), true, true);
            Log.e(TAG, "fx---->WeatherAidlService sendParseResult"+jsonDataString.toString());
            sendParseResult(requestData, jsonDataString);
        }

        @Override
        public void registerCallBack(IRequestCallBack callback, String packageName)
                throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            if (null != callback && !mCallbackList.containsKey(packageName)) {
                HwLog.d(TAG, "Register packageName = " + packageName);
                Log.e(TAG, "fx---->WeatherAidlService Register packageName = " + packageName);
                mCallbackList.put(packageName, callback);
            }
        }

        @Override
        public void unregisterCallBack(IRequestCallBack callback, String packageName)
                throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            if (null != callback && mCallbackList.containsKey(packageName)) {
                HwLog.d(TAG, "Unregister packageName = " + packageName);
                Log.e(TAG, "fx---->WeatherAidlService Register unregisterCallBack = " + packageName);
                mCallbackList.remove(packageName);
            }
        }

        @Override
        public void requestWeatherByLocationAndSourceType(
                RequestData requestData, int type) throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            HwLog.d(TAG, "requestWeatherByLocationAndSourceType->data source type:" + type);
            if(isRequestDataWithGeoPosInValidate(requestData)) {
                HwLog.w(TAG, "requestWeatherByLocationAndSourceType->request data is invalidate");
                sendParseResult(requestData, PARSE_ERROR_RESULT);
                return;
            }
            WeatherAsyncTask task = new WeatherWithDadaSourceTypeAsyncTask(requestData, type);
            task.execute(createWeatherTaskInfoBasedOnRequest(requestData));
        }

        @Override
        public void requestWeatherWithLocation(RequestData requestData, int sourceType,
                int parsePhaseType) throws RemoteException {
//            enforceCallingOrSelfPermission(THIRD_REQUEST_PERMISSION, null);
            HwLog.d(TAG, "requestWeather->data source type:" + sourceType +
                    ", parsePhaseType:" + parsePhaseType);
            if(isRequestDataWithGeoPosInValidate(requestData)) {
                HwLog.w(TAG, "requestWeatherByLocationAndSourceType->request data is invalidate");
                sendParseResult(requestData, PARSE_ERROR_RESULT);
                return;
            }
            WeatherAsyncTask task = new WeatherWithSourceAndPhaseTypeAsyncTask(
                    requestData, sourceType, parsePhaseType);
            task.execute(createWeatherTaskInfoBasedOnRequest(requestData));
        }
    };

    private boolean isRequestDataWithGeoPosInValidate(RequestData requestData) {
        return requestData == null || !TotemLocation.isValidLocaiton(
                    requestData.getmLongitude(), requestData.getmLatitude());
    }

    private boolean isRequestMyPosWeather(RequestData requestData) {
        final float MAX_DIFFER = 0.01f;
        LocationResult curPos = HwLocationManager.getInstance().getResult();
        if(null == curPos) {
            HwLog.d(TAG, "isRequestMyPosWeather->there is no my position");//TODO:add radar
            return false;
        }
        return Math.abs(curPos.mLat - requestData.getmLatitude()) < MAX_DIFFER
                && Math.abs(curPos.mLon - requestData.getmLongitude()) < MAX_DIFFER;
    }

    private class WeatherWithSourceAndPhaseTypeAsyncTask extends
            WeatherWithDadaSourceTypeAsyncTask {
        protected int mParsePhaseType;
        public WeatherWithSourceAndPhaseTypeAsyncTask(RequestData requestData,
                int dataSourceType, int parsePhaseType) {
            super(requestData, dataSourceType);
            mParsePhaseType = parsePhaseType;
        }

        @Override
        protected WeatherInfo parseWeatherFromNetwork(WeatherTaskInfo taskInfo) {
            return WeatherTaskController.getInstance(
                    WeatherAidlService.this).handleTaskImpl(
                        taskInfo, mDataSourceType, mParsePhaseType);
        }
    }

    private class WeatherWithDadaSourceTypeAsyncTask extends WeatherAsyncTask {

        protected int mDataSourceType;

        public WeatherWithDadaSourceTypeAsyncTask(RequestData requestData, int dataSourceType) {
            super(requestData);
            mDataSourceType = dataSourceType;
        }

        @Override
        protected WeatherInfo parseWeatherInfo(WeatherTaskInfo taskInfo) {
            WeatherInfo weather = tryToReturnWeatherInfoInDatabase();
            return weather != null ? weather: parseWeatherFromNetwork(taskInfo);
        }

        protected WeatherInfo parseWeatherFromNetwork(WeatherTaskInfo taskInfo) {
            return WeatherTaskController.getInstance(
                    WeatherAidlService.this).handleTaskImpl(taskInfo, mDataSourceType);
        }

        protected WeatherInfo tryToReturnWeatherInfoInDatabase() {
            //return database weather if the specified datasource type is
            //the same with current type
            if(Utils.getCurrentDataSourceType(WeatherAidlService.this) == mDataSourceType
                    && isRequestMyPosWeather(mRequestData)) {
                CityInfo myCityInfo = queryLocationCityInfo();
                WeatherInfo weather = queryWeatherInfo(myCityInfo);
                final long OUTDATE_TIME = 3600000;//1 hour
                if(System.currentTimeMillis() - weather.mTime < OUTDATE_TIME) {
                    HwLog.d(TAG, "parseWeatherInfo->return weather from database");
                    return weather;
                }
            }
            return null;
        }
    }

    private class WeatherAsyncTask extends AsyncTask<WeatherTaskInfo, WeatherTaskInfo, String>{
        protected RequestData mRequestData;

        public WeatherAsyncTask(RequestData requestData){
            mRequestData = requestData;
        }

        protected boolean isTaskInfoParamsInValidate(WeatherTaskInfo[] taskInfos) {
            return null == taskInfos || taskInfos.length < 1;
        }

        protected WeatherInfo parseWeatherInfo(WeatherTaskInfo taskInfo) {
            return WeatherTaskController.getInstance(WeatherAidlService.this)
                    .handleTaskImpl(taskInfo);
        }

        @Override
        protected String doInBackground(WeatherTaskInfo... taskInfos) {
            
            Log.e(TAG, "fx----> WeatherAidlService taskInfos : "+taskInfos.toString());
            Log.e(TAG, "fx----> WeatherAidlService isTaskInfoParamsInValidate : "+isTaskInfoParamsInValidate(taskInfos));
            if(isTaskInfoParamsInValidate(taskInfos)){
                HwLog.w(TAG, "WeatherAsyncTask->doInBackground->taskInfos invalidate");
                return null;
            }
            Log.e(TAG, "fx----> WeatherAidlService taskInfo : "+taskInfos[0].toString());
            WeatherInfo weatherInfo = parseWeatherInfo(taskInfos[0]);
            Log.e(TAG, "fx----> WeatherAidlService weatherInfo : "+weatherInfo.toString());
            if (null == weatherInfo) {
                Log.e(TAG, "fx----> WeatherAidlService weatherInfo is null ");
                HwLog.w(TAG, "WeatherAsyncTask->doInBackground->weatherInfo is null");
                return null;
            }

            final CityInfo cityInfo = new CityInfo();
            //Log.i(TAG, "weatherInfo = " + weatherInfo);/for test
            cityInfo.updateCityInfo(WeatherAidlService.this,weatherInfo);
            Utils.dealCityInfoWeatherInfo(WeatherAidlService.this, cityInfo, weatherInfo);
            BaseInfoUtils.setWeatherId(weatherInfo, BaseInfoUtils.getWeatherId(cityInfo));

            BaseInfoUtils.setWeatherStatus(weatherInfo, WeatherInfo.STATUS_DATA_OK);
            if (null != weatherInfo.mWeatherAlarms &&
                    weatherInfo.mWeatherAlarms.size() >= WeatherAlarm.SECOND_ALARM) {
                WeatherAlarm.sort(weatherInfo.mWeatherAlarms);
            }

            Log.e(TAG, "fx----> WeatherAidlService return : "+HomeCityWeather.packJsonData(WeatherAidlService.this, cityInfo,
                    weatherInfo.clone(), mRequestData.ismAllDay(), true, false));
            
            return HomeCityWeather.packJsonData(WeatherAidlService.this, cityInfo,
                    weatherInfo.clone(), mRequestData.ismAllDay(), true, false);
        }

        @Override
        protected void onPostExecute(String result) {
            Log.e(TAG, "fx---->WeatherAidlService task onPostExecute:: "+result);
            if(TextUtils.isEmpty(result)) {
                result = PARSE_ERROR_RESULT;
                HwLog.w(TAG, "onPostExecute->parse result is empty");
                Log.e(TAG, "fx---->WeatherAidlService task ->parse result is empty ");
            }
            sendParseResult(mRequestData, result);
        }
    }

    private WeatherTaskInfo createWeatherTaskInfoBasedOnRequest(
            RequestData requestData) {
        CityInfo cityInfo = new CityInfo(CityInfo.CITY_TYPE_MY_LOCATION);
        WeatherTaskInfo info = new WeatherTaskInfo(cityInfo);
        info.setGeoPosition(requestData.getmLongitude(), requestData.getmLatitude());
        info.setTaskState(WeatherTaskInfo.WEATHER_TASK_LOCATIED_SUCCESS);
        info.indicateToOutSideLocateTask();
        Log.e(TAG, "fx----> WeatherTaskInfo:"+info.toString());
        return info;
    }

    private void sendParseResult(RequestData requestData, String parseResult) {
        Log.e(TAG, "fx----> WeatherAidlService parseResult :" +parseResult);
        if (null == requestData) {
            Log.e(TAG, "fx---->WeatherAidlService requestData == null");
            HwLog.d(TAG, "sendParseResult requestData = null");
            requestData = new RequestData();
        }

        if (mCallbackList.containsKey(requestData.getmPackageName())) {
            try {
                HwLog.d(TAG, "onRequestResult");
                Log.e(TAG, "fx---->WeatherAidlService getmPackageName 2 :" +requestData.getmPackageName());
                IRequestCallBack callBack = mCallbackList.get(requestData.getmPackageName());
                Log.e(TAG, "fx---->WeatherAidlService parseResult 2 :" +parseResult);
                callBack.onRequestResult(parseResult, requestData);
                
            } catch (RemoteException e) {
                HwLog.e(TAG, "RemoteException >> " + e);
                Log.e(TAG, "fx---->WeatherAidlService RemoteException " + e);
            }
        }else {
            Log.e(TAG, "fx---->WeatherAidlService mCallbackList :" +mCallbackList.toString());
            Log.e(TAG, "fx---->WeatherAidlService requestData.getmPackageName() :" +requestData.getmPackageName());
        }
    }

    protected CityInfo queryLocationCityInfo(){
        return mWeatherDataManager.queryLocationCityInfo();
    }

    protected WeatherInfo queryWeatherInfo(CityInfo cityInfo){
        return mWeatherDataManager.queryWeatherInfo( cityInfo);
    }

    private CityInfo getHomeCityOrMyLocation(){
        CityInfo cityInfo = mWeatherDataManager.queryHomeCityInfo();
        if(null == cityInfo){
            cityInfo = mWeatherDataManager.queryLocationCityInfo();
        }
        return cityInfo;
    }

    private CityInfo getMyLocationOrHomeCity(){
        return mWeatherDataManager.queryDefaultCityInfo();
    }
}

/////////////////////////////////////////////////
// 客户端代码 AIDL文件 文件路径必须和服务端一致 .java
package com.huawei.android.totemweather.aidl;

import android.content.Context;
import android.os.Parcel;
import android.os.Parcelable;

public class RequestData implements Parcelable {

    /** application package name */
    private String mPackageName;
    /** request flag */
    private String mRequesetFlag;
    /** form : beijing -> "cityId:101010100" , New York -> "cityId:USNY0996" */
    private String mCityId;
    /** location latitude */
    private double mLatitude;
    /** location longitude */
    private double mLongitude;
    /**
     * request city weather type. see {@link #TYPE_MY_LOCATION} and
     * {@link #TYPE_HOME_CITY}
     */
    private int mCityType = TYPE_HOME_CITY;
    /** all future forecast weather, or one day weather */
    private boolean mAllDay = true;

    /** my location city type */
    public static final int TYPE_MY_LOCATION = 1;
    /** home city type */
    public static final int TYPE_HOME_CITY = 2;
    /**
     * first return home city, return my location if home city not exists
     */
    public static final int TYPE_HOME_CITY_FIRST = 3;
    /**
     * first return my location, return home city if my location not exists
     */
    public static final int TYPE_MY_LOCATION_FIRST = 4;
    public RequestData() {
    }

    public RequestData(Parcel in) {
        readFromParcel(in);
    }

    /**
     * use this constructor when you use
     * {@link com.huawei.android.totemweather.aidl.IRequestCityWeather#requestWeatherByLocation(RequestData)}
     *
     * @param context Context
     * @param latitude location latitude
     * @param longitude location longitude
     */
    public RequestData(Context context, double latitude, double longitude) {
        mPackageName = context.getPackageName();
        mRequesetFlag = latitude + "," + longitude;
        mLatitude = latitude;
        mLongitude = longitude;

    }

    /**
     * use this constructor when you use
     * {@link com.huawei.android.totemweather.aidl.IRequestCityWeather#requestWeatherByCityId(RequestData)}
     *
     * @param context Context
     * @param cityId form : beiJing -> "cityId:101010100" , New York ->
     *            "cityId:USNY0996"
     */
    public RequestData(Context context, String cityId) {
        mPackageName = context.getPackageName();
        mRequesetFlag = cityId;
        mCityId = cityId;
    }

    /**
     * use this constructor when you use
     * {@link com.huawei.android.totemweather.aidl.IRequestCityWeather#getWeatherByType(RequestData)}
     *
     * @param context
     *            Context
     * @param cityType request city weather type. see {@link #TYPE_MY_LOCATION} and {@link #TYPE_HOME_CITY}
     */
    public RequestData(Context context, int cityType) {
        mPackageName = context.getPackageName();
        mRequesetFlag = cityType + "";
        mCityType = cityType;
    }

    public String getmPackageName() {
        return mPackageName;
    }

    public void setmPackageName(String mPackageName) {
        this.mPackageName = mPackageName;
    }

    public String getmRequesetFlag() {
        return mRequesetFlag;
    }

    public void setmRequesetFlag(String mRequesetFlag) {
        this.mRequesetFlag = mRequesetFlag;
    }

    public String getmCityId() {
        return mCityId;
    }

    public void setmCityId(String mCityId) {
        this.mCityId = mCityId;
    }

    public double getmLatitude() {
        return mLatitude;
    }

    public void setmLatitude(double mLatitude) {
        this.mLatitude = mLatitude;
    }

    public double getmLongitude() {
        return mLongitude;
    }

    public void setmLongitude(double mLongitude) {
        this.mLongitude = mLongitude;
    }

    public int getmCityType() {
        return mCityType;
    }

    public void setmCityType(int mCityType) {
        this.mCityType = mCityType;
    }

    public boolean ismAllDay() {
        return mAllDay;
    }

    public void setmAllDay(boolean mAllDay) {
        this.mAllDay = mAllDay;
    }

    @Override
    public int describeContents() {
        return 0;
    }

    public void readFromParcel(Parcel in) {
        mPackageName = in.readString();
        mRequesetFlag = in.readString();
        mCityId = in.readString();
        mLatitude = in.readDouble();
        mLongitude = in.readDouble();
        mCityType = in.readInt();
        mAllDay = in.readInt() == 1;

    }

    @Override
    public void writeToParcel(Parcel dest, int flags) {
        dest.writeString(mPackageName);
        dest.writeString(mRequesetFlag);
        dest.writeString(mCityId);
        dest.writeDouble(mLatitude);
        dest.writeDouble(mLongitude);
        dest.writeInt(mCityType);
        dest.writeInt(mAllDay ? 1 : 0);
    }

    public static final Parcelable.Creator<RequestData> CREATOR = new Parcelable.Creator<RequestData>() {
        public RequestData createFromParcel(Parcel p) {
            return new RequestData(p);
        }

        public RequestData[] newArray(int size) {
            return new RequestData[size];
        }
    };

    @Override
    public String toString() {
        return "RequestData [mPackageName=" + mPackageName + ", mRequesetFlag="
                + mRequesetFlag + ", mCityId=" + mCityId + ", mCityType="
                + mCityType + ", mAllDay=" + mAllDay + "]";
    }



}
///////////////////////////////////////.xml
<?xml version="1.0" encoding="utf-8"?>


<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.android.clientApp"
    android:sharedUserLabel="@string/app_label"
    android:versionCode="50000001"
    android:versionName="5.0.0.2" >

   <!-- 关键代码 由于对方的AIDLservice加了此权限，因此客户端需要在此声明此权限-->
    <uses-permission android:name="com.example.android.testapp.permission.ACCESS_WEATHERCLOCK_PROVIDER"></uses-permission>
   
    <application
        android:name="CalendarApplication"
        android:backupAgent="com.android.clientApp.CalendarBackupAgent"
        android:hardwareAccelerated="true"
        android:icon="@drawable/ic_launcher_icon"
        android:label="@string/app_label"
        android:supportsRtl="true"
        android:multiArch="true"
        android:allowBackup="false"
        android:taskAffinity="android.task.clientApp" >
        
       
    </application>

</manifest>

/////////////////////////////////////////////////////////////服务端代码
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.android.testapp"
    android:versionCode="610011"
    android:versionName="6.1.11" >
    
	<!-- 关键代码 permission标签都是自定义权限 android:protectionLevel="signatureOrSystem"是安全等级-->
    <permission
        android:name="com.example.testapp.permission.THIRD_REQUEST_WEATHER"
        android:protectionLevel="signatureOrSystem" />
    <permission
        android:name="com.example.android.testapp.permission.ACCESS_WEATHERCLOCK_PROVIDER"
        android:protectionLevel="signatureOrSystem" />
    <uses-permission android:name="com.example.testapp.permission.THIRD_REQUEST_WEATHER" />
  
    <application
        android:name="TestApp"
        android:allowBackup="false"
        android:defaultToDeviceProtectedStorage="true"
        android:directBootAware="true"
        android:hardwareAccelerated="false"
        android:icon="@drawable/ic_launcher_icon"
        android:label="@string/app_name_a"
        android:supportsRtl="true"
        android:theme="@android:style/Theme.Holo.Light" >
        

       <!-- 关键代码  带了自定义权限的service，意味着第三方APP在访问此service的时候需要在manifest里面注册相同的权限-->
        <service
            android:name=".aidl.WeatherAidlService"
            android:enabled="true" 
            android:exported="true" 
            android:permission="com.example.android.testapp.permission.ACCESS_WEATHERCLOCK_PROVIDER"
            >
            <intent-filter>
                <action android:name="com.example.testapp.action.THIRD_REQUEST_WEATHER" />
            </intent-filter>
        </service>

      
    </application>

</manifest>
